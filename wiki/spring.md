---
creationDate        : 2004-08-30 14:31:47 +0200 
author              : kocka 
title               : Spring Framework 
name                : spring 
layout              : wiki 
path                : spring 
date                : 2008-03-12 13:10:12 +0100 
version             : 19 
creator             : kocka 
---
__[TODO](TODO.html): ez a snip megérett egy alapos átírásra.__

![image](http://www.springframework.org/docs/reference/images/spring-overview.gif)

## Spring IOC

A Spring framework lelke az [IoC](ioc.html) container. Nem intrusiv, azaz kb bármi lehet spring bean, például egy [dbcp](DBCP.html) datasource, aminek semmi kötődése nincs a springhez. így bármilyen [POJO](pojo.html) lehet spring komponens.

A [lifecycle](lifecycle.html)-hez vagy használ az ember Spring-specifikus interfaceket, vagy meghatározhat metódusokat amiket a container meghív a kellő fázisban.

Mind getter-setter, mind pedig konstruktor alapú [IoC](ioc.html) támogatja, valamint factory-nak is fel lehet használni szinte bármit annélkül hogy speciális interfacet implementálni kellene. 

A komponenseket az alkalmazáskontextben lehet összekötni egy alkalmazássá, ez többnyire egy XML.

## Spring [Web alkalmazásokhoz](webapp.html)

A Spring az alábbiakkal támogatja a webalkalmazások fejleszését:

*   Spring Web [MVC](MVC.html), XML-el konfiguralhato [MVC](MVC.html), tamogatas kulombozo View retegek fele ([PDF](PDF.html), [Velocity](Velocity.html), [JSP](JSP.html)...)
*   Spring Web framework, [XML](XML.html)-el konfiguralhato Web context
*   Integráció más web frameworkökkel: [Tapestry](tapestry.html), [struts](struts.html), [jsf](JSF.html) ésatöbbi...
*   Viszonylag új még a Spring WS, a [Web Services](Missing.html) subproject.

## Spring [JMS](JMS.html)


## Spring ORM

*   [hibernate](Hibernate.html), [jdo](JDO.html), [jdbc](JDBC.html) support a híres templates megoldással vagy nélküle.
*   [JPA](JPA.html) support is van már

## [IDE](IDE.html) támogatás

Ez nem szükséges egy springes fejlesztéshez, de tud segíteni olyanokban mint a context xml-el szerkesztése, web flow diagrammok, stb...
Az [eclipse](Eclipse.html) [plugin](http://springide.org/) 2.0ás verziójáról egy cikk: [Introducing Spring IDE 2.0](http://www.javabeat.net/articles/2007/09/introduction-to-spring-ide-2-0/5)

## Spring és [unit-tesztelés](test.html)

Korábban is elterjedt megoldás volt az, hogy a tesztelendő POJO létrehozását és inicializációját a spring-re bízta egy unit teszt. Erre mindenkinek megvolt a saját kis megoldása. Figyelemre méltó viszont a [unitils](Unitils.html) spring támogatása, amiben csak [annotiációkkal](annotations.html) megmondhatjuk hogy melyik XML-ből jöjjön létre az alkalmazás context, és melyik bean-ek hova injektálódjanak be.

## Külső, kapcsolódó projectek

*   security: [acegi](acegi.html)

## Cikkek, linkek

1.1.1 Cikkek:

*   [What's New in Spring 2.5: Part 1](http://www.infoq.com/articles/spring-2.5-part-1)
*   [Why Spring JDBC?](http://today.java.net/pub/a/today/2006/05/09/why-spring-jdbc.html)

1.1.1 Linkek:

*   [Spring weboldal](http://www.springframework.org/)
*   [Spring HUB](http://springhub.com/)



