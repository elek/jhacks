---
creationDate        : 2005-03-15 15:46:38 +0100 
author              : admin 
title               : quartz 
name                : quartz 
layout              : wiki 
path                : quartz 
date                : 2006-03-26 01:48:39 +0100 
version             : 1 
creator             : kocka 
---
![image](http://www.opensymphony.com/quartz/images/quartzEJS.jpg)<br/>
[http://www.opensymphony.com/quartz/](http://www.opensymphony.com/quartz/)

Job scheduler [J2EE](j2ee.html) ([EJB](EJB.html) vagy egyszeruen csak [cop](COP.html) rendszerekhez). Ezen a teren nagyjabol egyeduralkodo.

Nagyon sok felhasznalojuk van es a [spring](spring.html) framework is integralja magaba. Egy atlagos schedulertol abban is kulonbozik hogy sajat persistence rendszere van, azaz tehetsz moge akar egy [RDBMS](RDBMS.html)t is ahol tarolhatja a jobokat. Aminek persze megvan a maga kenyelmes es kevesbe kenyelmes oldala. Pl mar letezo schedulerek lehelyettesitesere annyir nem jo, uj architekturaba viszont eleg fullos megoldas.

Egy kis tortenelem: regebben hasznaltam a [harvest](harvest.html)ben egy [avalon](avalon.html)os komponenst, ami akkoriban tok jo otletnek tunt, es jol is ment, semmi bajom nem volt vele. Miota visszont az [avalon](avalon.html) [deprecated](deprecated.html), egyre tobbszor merult fel az igeny hogy az alkalmazasaimat fuggetlenitsem tole. Es ekkor jott a pofon, hogy az a scheduler amit en hasznaltam, az ugy hozza volt drotozva az [avalon](avalon.html)hoz hogy el se lehetett tole valasztani.

Ugyhogy javaslom elovigyazatossagbol csak [pojo](pojo.html) alapu komponenseket valogassatok be, es schedulerbol a quartz tenyleg jo.
