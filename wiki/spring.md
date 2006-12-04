---
creationDate        : 2004-08-30 14:31:47 +0200 
author              : kocka 
title               : spring 
name                : spring 
layout              : wiki 
path                : spring 
date                : 2006-12-04 17:43:50 +0100 
version             : 10 
creator             : kocka 
---
__Spring Framework__

A Spring framework egy "komplex" joszag.Legyen itt lathato egy kisebb elemzes
Az alabbi abra jol szemlelteti a felepiteset:

[Spring felepitese](http://www.springframework.org/docs/reference/images/spring-overview.gif)

A Spring alapvetoen JavaBeanekkel (ertsd: [POJO](pojo.html)) dolgozik, igy nincs szukseg a "koltseges" [J2EE](j2ee.html) kontenerekre (melyek eroforras igenye igen csak nagy). Webes megjeleneshez eleg egy egyszeru java alapu webszerver (pl.: Jetty/Tomcat). Funkcionalitasaban joval megelozi az [EJB](EJB.html)-t.

Nehany fontosabb tulajdonsaga:

*   Spring [AOP](AOP.html) kontener , [XML](XML.html)-bol vezerlheto [AOP](AOP.html) kontenerre rendelkezik, mellyel az AOP hivasok keszitese lenyegessen leegyszerusodik
*   [IoC](ioc.html) kontener, Inversion of Control kontenert tartalmaz, ezaltal [XML](XML.html)-en keresztul allithatoak be az egyes Bean-ek kapcsolatai (Mivel JavaBeaneket hasznal igy az [IoC](ioc.html) a setter es getter metodusokon keresztul illetve (csunyabb megoldaskent) a kontruktoron keresztul tudja az adott osztalynak atadni a tobbi Bean-t)
*   Spring [OR Mapping](OR%20Mapping.html) (ORM), [XML](XML.html) alapu beallitas tobb fele ORM fele ([Hibernate](Hibernate.html),[JDO](JDO.html),iBatis)
*   Spring [DAO](DAO.html), szinten [XML](XML.html)-en keresztul konfiguralhato tranzakcio kezeles, [JDBC](JDBC.html) es [DAO](DAO.html) tamogatas
*   Spring Web framework, [XML](XML.html)-el konfiguralhato Web context
*   Spring Web [MVC](MVC.html), XML-el konfiguralhato [MVC](MVC.html), tamogatas kulombozo View retegek fele ([PDF](PDF.html), [Velocity](Velocity.html), [JSP](JSP.html)...)
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


