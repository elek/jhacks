---
creationDate        : 2004-08-30 14:31:47 +0200 
author              : kocka 
title               : Spring Framework 
name                : spring 
layout              : wiki 
path                : spring 
date                : 2008-03-11 13:13:04 +0100 
version             : 17 
creator             : kocka 
---
__[TODO](TODO.html): ez a snip megérett egy alapos átírásra.__

![image](http://www.springframework.org/docs/reference/images/spring-overview.gif)

## Spring IOC

A Spring framework lelke az [IoC](ioc.html) container. Nem intrusiv, azaz kb bármi lehet spring bean, például egy [dbcp](DBCP.html) datasource, aminek semmi kötődése nincs a springhez.
A lifecycle-hez vagy használ az ember Spring-specifikus interfaceket, vagy meghatározhat metódusokat amiket a container meghív a kellő fázisban.
Mind getter-setter, mind pedig konstruktor alapú [IoC](ioc.html) támogatja, valamint factory-nak is fel lehet használni szinte bármit annélkül hogy speciális interfacet implementálni kellene.

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
Az [eclipse](Eclipse.html) plugin 2.0ás verziójáról egy cikk: [Introducing Spring IDE 2.0](http://www.javabeat.net/articles/2007/09/introduction-to-spring-ide-2-0/5)

## Spring és [unit-tesztelés](test.html)

Korábban is elterjedt megoldás volt az, hogy a tesztelendő POJO létrehozását és inicializációját a spring-re bízta egy unit teszt. Erre mindenkinek megvolt a saját kis megoldása. Figyelemre méltó viszont a [unitils](Unitils.html) spring támogatása, amiben csak [annotiációkkal](annotations.html) megmondhatjuk hogy melyik XML-ből jöjjön létre az alkalmazás context, és melyik bean-ek hova injektálódjanak be.

## Cikkek


*   [What's New in Spring 2.5: Part 1](http://www.infoq.com/articles/spring-2.5-part-1)




== régi tartalom ==

A Spring framework egy "komplex" joszag.Legyen itt lathato egy kisebb elemzes
Az alabbi abra jol szemlelteti a felepiteset:

[Spring felepitese](http://www.springframework.org/docs/reference/images/spring-overview.gif)

A Spring alapvetoen JavaBeanekkel (ertsd: [POJO](pojo.html)) dolgozik, igy nincs szukseg a "koltseges" [J2EE](j2ee.html) kontenerekre (melyek eroforras igenye igen csak nagy). Webes megjeleneshez eleg egy egyszeru java alapu webszerver (pl.: Jetty/Tomcat).

Nehany fontosabb tulajdonsaga:

*   Spring [AOP](AOP.html) kontener , [XML](XML.html)-bol vezerlheto [AOP](AOP.html) kontenerre rendelkezik, mellyel az AOP hivasok keszitese lenyegessen leegyszerusodik
*   [IoC](ioc.html) kontener, Inversion of Control kontenert tartalmaz, ezaltal [XML](XML.html)-en keresztul allithatoak be az egyes Bean-ek kapcsolatai (Mivel JavaBeaneket hasznal igy az [IoC](ioc.html) a setter es getter metodusokon keresztul illetve (csunyabb megoldaskent) a kontruktoron keresztul tudja az adott osztalynak atadni a tobbi Bean-t)
*   Spring [OR Mapping](OR%20Mapping.html) (ORM), [XML](XML.html) alapu beallitas tobb fele ORM fele ([Hibernate](Hibernate.html),[JDO](JDO.html),iBatis)
*   Spring [DAO](DAO.html), szinten [XML](XML.html)-en keresztul konfiguralhato tranzakcio kezeles, [JDBC](JDBC.html) es [DAO](DAO.html) tamogatas
*   Rendelkezik tamogatassal [EJB](EJB.html), [WebServices](WebServices.html), [RMI](RMI.html), [JMS](JMS.html) illetve [JavaMail](Missing.html) fele.
*   Atlathato (XML konfiguracionak hala)
*   Gyors (leven hogy nemkell a nagy eroforras igenyu [J2EE](j2ee.html) kontener)
*   Alkalmas mind weblapok mind alkalmazasok keszitesere
*   [Hibernate](Hibernate.html) tamogatasnak koszonhetoen teljessen letudja valtani az [EJB](EJB.html) [CMP](CMP.html) Beaneket.
*   [lifecycle](lifecycle.html): ezt a spring is sajat interfacekkel implementalja, azaz spring fuggove valik a bean-ed.
*   security: [acegi](acegi.html)

Igy tomoren ennyi. Nagyon jol hasznalhato Framework, akar application akar weblap keszitesrol legyen szo, barmelyik teruleten jol hasznalhato. Mas [webapp](webapp.html) frameworkok is integralva vannak hozza: [struts](struts.html), [webwork](WebWork.html), satobbi(sikerult [laszlo](Laszlo.html)t is integralni de ez nem volt olyan ecceru eset :))
. Ez ugy mukodik, hogy a [web.xml](Missing.html)-ben definialsz egy springes listenert ami elinditja a spring rendszert es beregisztralja a [servlet](servlet.html) contextedbe. Ezutan akarmalyik komponensnek szuksege van ra, innen veheti ki, de erre azert az alkalmazaskomponenseknek nincs nagyon szukseguk :)
Linkek:

*   [Spring weboldal](http://www.springframework.org/)
*   [Spring HUB](http://springhub.com/)
*   [Why Spring JDBC?](http://today.java.net/pub/a/today/2006/05/09/why-spring-jdbc.html)
*   [IDE](IDE.html) support: [eclipse](Eclipse.html)hez: [http://springide.org/](http://springide.org/)



