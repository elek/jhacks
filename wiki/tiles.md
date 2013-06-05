---
creationDate: 1134649921507 
author: kocka 
contentAuthor: kocka 
title: Tiles 
contentUpdateDate: 1194959799054 
name: tiles 
layout: wiki 
date: 1194959799054 
creator: kocka 
---
http://tiles.apache.org/

Egy szerver oldali UI komponens rendszer.
Na, szóval amit a [tapestry](tapestry.html) komponensnek nevez, az itt tile.

## Történet

A tiles a [struts 1-el](struts/struts%201.html) indult, majd a [struts/struts 2](struts/struts%202.html) már nélküle jött ki, és külön topp level [apache](ASF.html) projectet kapott a cucc.

1.1.1 Struts tiles

Valahogy ennyi az egesz: egy [xml](XML.html)ben definialod hogy milyen darabokbol all a view, es ezekhez rendelsz [jsp](JSP.html)-ket. Ez hierarchikusan is megy, azaz pl definialsz egy alap komponenst ami a headert meg a footert deklaralja, es a tobbi leszarmaztatott meg tudja hogy mi a content.

A view darabokhoz definialhatsz egy controllert is, ez egy koddarab ami lefut mielott a jsp megkapna a vezerlest, es pl betoltheti a szukseges adatokat. a ami viszont faj: A [jsp](JSP.html)ben kell meghatarozni hogy melyik az az osztaly, nem deklaracios [xml](XML.html)ben.

Meg persze tartoznak hozza [jsp](JSP.html) tagek, amivel lehet include-olni. Vegulis ennyivel ubereli a [jsp](JSP.html) include csodajat. Amivel alulmulja az az hogy a beinclude-olt jsp-bol mar ugyanigy tiles-szal nem lehet masikat betolteni, szoval igy nem hierarchikus.

Szoval egy alapvetoen jo otlet, csak sok vele a szopas :(

Had tegyem kozze [gonosz](gonosz.html) osztalyomat amivel [spring](spring.html) contextben regisztralhatod a controller beanjeidet, igy nem kell a [spring](spring.html)es applicationcontext-bol bogarasznod ki a szukseges ban-eket, hanem hasznalhatod a setter vagy konstruktor alapu [dependency injection](dependency%20injection.html)t.

{% highlight java %}

import javax.servlet.ServletContext;
import javax.servlet.ServletRequest;

import org.apache.log4j.Logger;
import org.apache.struts.tiles.ComponentDefinition;
import org.apache.struts.tiles.Controller;
import org.apache.struts.tiles.DefinitionsFactoryException;
import org.apache.struts.tiles.NoSuchDefinitionException;
import org.apache.struts.tiles.xmlDefinition.I18nFactorySet;
import org.springframework.context.ApplicationContext;
import org.springframework.web.context.support.WebApplicationContextUtils;

/**
 * This is a hack around the tiles architecture, so that one can register controller beans in spring.
 * 
 * @author kocka
 */
public class SpringDefinitionsFactory 
		extends I18nFactorySet \{

	Logger logger = Logger.getLogger(SpringDefinitionsFactory.class);
	
	/* (non-Javadoc)
	 * @see org.apache.struts.tiles.DefinitionsFactory#getDefinition(java.lang.String, javax.servlet.ServletRequest, javax.servlet.ServletContext)
	 */
	public ComponentDefinition getDefinition(String name,
			ServletRequest request, ServletContext servletContext)
			throws NoSuchDefinitionException, DefinitionsFactoryException \{
		if(logger.isDebugEnabled())
			logger.debug("requested definition of "+name);

		ApplicationContext context = WebApplicationContextUtils.getWebApplicationContext(servletContext);
		ComponentDefinition def = super.getDefinition(name, request, servletContext);
		if(def != null)\{
			String controller = def.getController();
			Controller controllerInstance = def.getControllerInstance();
			if(controllerInstance == null && controller != null)\{
				controllerInstance = (Controller) context.getBean(controller);
				def.setControllerInstance(controllerInstance);
			\}
		\}
		return def;
	\}

\}

{% endhighlight %}


1.1.1 Apache Tiles

Top level project, elvileg független a [strutstól](struts.html)
