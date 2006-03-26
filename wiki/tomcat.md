---
creationDate        : 2004-08-04 10:46:30 +0200 
author              : admin 
title               : tomcat 
name                : tomcat 
layout              : wiki 
path                : tomcat 
date                : 2006-03-26 01:51:20 +0100 
version             : 1 
creator             : kocka 
---
![image](http://tomcat.apache.org/images/tomcat.gif)(http://tomcat.apache.org/)

A tomcat az [ASF](ASF.html) [servlet](servlet.html) es [jsp](JSP.html) szervere. Az egyik legnepszerubb szoftver a kategoriaban.

Amit tudni kell rola: egy jo ideig a SUN refrencia implementacioja volt a [Servlet_jsp](servlet_jsp.html) temakoreben. Ha csak erre a kettore van szukseged, akkor erdemes ot valasztani. Gyors, egyszeru. Fut Windows es Linux alatt is, sok szep funkcioja van. Konnyu telepiteni.

A tomcat nem egy komplett [j2ee](j2ee.html) [alkalmazas szerver](Alkalmazas%20Szerver.html), hanem csak egy web container. Ha szukseged van olyanokra mint [JTA](JTA.html), [EJB](EJB.html), [JMS](JMS.html), akkor vagy hasznalj egy elore osszeheggesztett [alkalmazas szerver](Alkalmazas%20Szerver.html)t vagy heggesz be a Tomcat-be mindenfele implementaciokat. Bar kihivasnak nyilvan az utobbi szebb, azert valoszinuleg fejdalom mentesebb az elobbi.<br/>
Azok az [alkalmazas szerver](Alkalmazas%20Szerver.html)ek, amibe tomcat van integralva: [jonas](jonas.html) [jboss](jboss.html)<br/>
(Szerintem a [jonas](jonas.html) nagyon rulez a management alkalmazasaval)

Nyilvan minek foglalja az eroforrast amit ugyse hasznalsz.
[Tyrex](tyrex.html)-hez es [OpenEJB](OpenEJB.html)-hez a weboldalon le van irva hogy kell integralni tomcatba.

__szopasok:___

A Tomcat erzekeny lelki vilagu allatfaj, konnyu megserteni konfiguralgatasok soran. Ha 500-at latsz a konfig kepernyon, akkor tudhatod hogy valami nagyon elszallt es jobb ha ujrainditod. Sokan javasoltak a [jetty](jetty.html)-t helyette.

Meg azt a nagyon baratsagos szoveget szeretem hogy "filterStart failed" ennyit hoz tudtodra akkor ha a filteredet nem tudta elinditani, semmi ok, vagy egy kedves kis stacktrace :) Persze emiatt az alkalmazasod se fog elindulni.

Linkek:

*   [tomcat website](http://tomcat.apache.org/)


Lasd: [clustering](Missing.html), [alkalmazas szerver](Alkalmazas%20Szerver.html)
