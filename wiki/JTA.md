---
creationDate: 1091019654598 
author: kocka 
contentAuthor: kocka 
title: JTA 
contentUpdateDate: 1105450313070 
name: JTA 
layout: wiki 
date: 1105450313070 
creator: kocka 
---
__Java Transaction Architecture__

http://java.sun.com/products/jta/

Szerveroldali tranzakciokezeles.

A JTA-ban a legjobb az, hogy szinte nem is kell vele foglalkozni, sot egy atlagos alkalmazas programozonak egyaltalan nem is kene. Persze alagos alkalmazas programozo valoszinuleg nincs ugyhogy nezzuk:

A JTA a thread-eddel asszocialja a tranzakciodat reprezentalo objektumot, amikor XADataSource implementaciokbol elkersz egy kapcsolatot, akkor abban mar ott a tranzakciod es te nem is hivhatsz commit() metodust, mert az nem a te hataskorod, hanem a tranzakcio vezerloe, amit az [alkalmazas szerver](Alkalmazas%20Szerver.html) szolgaltat.

Ez nagyon rulez akor amikor tobb adatforrasod es egyeb tranzakcionalis eroforrasod van, es szeretned ha konzisztensen kezelne oket a szoftvered.

Lasd: [JTS](JTS.html), [EJB](EJB.html), [JDBC](JDBC.html), [JavaMail](Missing.html), [JMS](JMS.html)
