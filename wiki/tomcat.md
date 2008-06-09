---
creationDate        : 2004-08-04 10:46:30 +0200 
author              : kocka 
title               : tomcat 
name                : tomcat 
layout              : wiki 
path                : tomcat 
date                : 2008-06-09 09:44:36 +0200 
version             : 11 
creator             : kocka 
---
![image](http://tomcat.apache.org/images/tomcat.gif)(http://tomcat.apache.org/)

# Tomi általában

A tomcat az [ASF](ASF.html) [servlet](servlet.html) es [jsp](JSP.html) szervere. Az egyik legnepszerubb szoftver a kategoriaban.

Amit tudni kell rola: egy jo ideig a SUN refrencia implementacioja volt a [Servlet_jsp](servlet_jsp.html) temakoreben. Ha csak erre a kettore van szukseged, akkor erdemes ot valasztani. Gyors, egyszeru. Fut Windows es Linux alatt is, sok szep funkcioja van. Konnyu telepiteni.

A tomcat nem egy komplett [j2ee](j2ee.html) [alkalmazas szerver](Alkalmazas%20Szerver.html), hanem csak egy web container. Ha szukseged van olyanokra mint [JTA](JTA.html), [EJB](EJB.html), [JMS](JMS.html), akkor vagy hasznalj egy elore osszeheggesztett [alkalmazas szerver](Alkalmazas%20Szerver.html)t vagy heggesz be a Tomcat-be mindenfele implementaciokat. Bar kihivasnak nyilvan az utobbi szebb, azert valoszinuleg fejdalom mentesebb az elobbi.<br/>
Azok az [alkalmazas szerver](Alkalmazas%20Szerver.html)ek, amibe tomcat van integralva: [jonas](jonas.html) [jboss](jboss.html) [geronimo](geronimo.html) [glassfish](glassfish.html) szoval majdnem minden...

Nyilvan minek foglalja az eroforrast amit ugyse hasznalsz.
[Tyrex](tyrex.html)-hez es [OpenEJB](OpenEJB.html)-hez a weboldalon le van irva hogy kell integralni tomcatba.

# Szívások

*   A Tomcat erzekeny lelki vilagu allatfaj, konnyu megserteni konfiguralgatasok soran. Ha 500-at latsz a konfig kepernyon, akkor tudhatod hogy valami nagyon elszallt es jobb ha ujrainditod. Sokan javasoltak a [jetty](jetty.html)-t helyette.

*   Meg azt a nagyon baratsagos szoveget szeretem hogy "filterStart failed" ennyit hoz tudtodra akkor ha a filteredet nem tudta elinditani, semmi ok, vagy egy kedves kis stacktrace :) Persze emiatt az alkalmazasod se fog elindulni.

*   [Cluster](cluster.html) téma... a 6.x-es szériában például a clusterdeployer törött, még a dokumentációja szerint is. Azért kis verekedés árán megy a dolog, de nem túl barátságos.

# Belső architektúra

Érdekes cucc belülről, egy pipeline-on megy végig a request, ennek a pipeline-nak a részei a valve-ok, ezek különböző dolgokat csinálhatnak a request továbbadása elött illetve után. Kicsit AOP feeling. Ilyenek vannak mint loging, stb...

Linkek:

*   [tomcat website](http://tomcat.apache.org/)


Lasd: [clustering](Missing.html), [alkalmazas szerver](Alkalmazas%20Szerver.html)
