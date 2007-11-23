---
creationDate        : 2004-07-28 13:01:44 +0200 
author              : kocka 
title               : geronimo 
name                : geronimo 
layout              : wiki 
path                : geronimo 
date                : 2007-11-23 13:41:08 +0100 
version             : 14 
creator             : kocka 
---
![image](http://www.epiqtech.com/corp/products/technology/opensource/images/design7_450x50.gif)(http://geronimo.apache.org/)

A geronimo az apache [j2ee](j2ee.html) [alkalmazas szerver](Alkalmazas%20Szerver.html)e. A komponens architekturajanak rugalmassagarol legendakat lehet hallani, valamint a [j2ee](j2ee.html) compliance teszten is atcsuszik (ez jelentjheti azt is hogy enterprise-ready ha gondolod, de lehet hogy nem ;) ). Nem csak egy [j2ee](j2ee.html) szerver, de egy nagyon felxibilis [IoC](ioc.html) container amibe konnyen lehet integralni barmit, ez egyebkent [jmx](JMX.html)-re epul, de alaposan kiegesziti a [jmx](JMX.html) architekturat.

Lasd meg:

*   [JMS](JMS.html): [ActiveMQ](ActiveMQ.html)
*   [EJB](EJB.html): [OpenEJB](OpenEJB.html)
*   [servlet](servlet.html): [jetty](jetty.html), [tomcat](tomcat.html)
*   egyeb cuccok: [spring](spring.html)

Geronimo ala konnyen lehet fejleszteni az [eclipse](Eclipse.html) [eclipse/plug-in/wtp](Eclipse/Plug-in/WTP.html) [eclipse/plug-in](Eclipse/Plug-in.html)-javal [webapp](webapp.html)okat, satobbit. Adminisztralni is egesz konnyen lehet az ujjabb 1.1-es verziot a konzol alkalmazasaval (szerintem kicsit [weblogic](weblogic.html) ihletesu, bar egyszerubb, de nagyon hasznos). A 2.X-es szeria mar jol boldogul a [java 1.5-tel](java%201.5.html).

Mókás kis dolog benne például az, hogy az összes megnyitott portot az alap konfig file egy kis properties fileban tartja, így nagyon könnyű több példányt feltelepíteni egy gépre, ráadásul kis offsetet is be lehet állítani. Ellenben más alkalmazás szerverekkel, ahol bogarászhatjuk végig a teljes konfigot. Szóval szép kis ötlet :)

Linkek:

*   [geronimo book](http://chariotsolutions.com/geronimo/)
*   Az [IBM](IBM.html) developerWorks [geronimo szekcioja](http://www-128.ibm.com/developerworks/opensource/top-projects/geronimo.html) egesz jo mellesleg...
*   [Onjava: What is geronimo?](http://www.onjava.com/lpt/a/6664)
*   [Geronimo wiki](http://cwiki.apache.org/geronimo/)


