---
creationDate: 1121245944292 
author: karenin 
contentAuthor: karenin 
title: Logging 
contentUpdateDate: 1203283138562 
name: Logging 
layout: wiki 
date: 1203283138562 
creator: kocka 
---
Java-hoz van tucat logging api, bar erdemes nem ezt hasznalni [debug](Missing.html)olas helyett :) de egy futo rendszer viselkedeset erdemes egy ilyen eszkozzel nyomonkovetni.

A regi szep idokben a [log4j](log4j.html) volt az egyeduralkodo, kozben mindenki irt valami custom baromsagot, nem mintha lenne benne nagy kihivas, es olyan elofordul hogy maga logging api okoz hibat. Feljott hat a [sun](Sun.html) is egy standard [java](java.html) logging apival ami resze a [j2sdk](Missing.html)nak. Igazabol meg senkit nem lattam hasznalni, de egyszer megneztem es olyan volt mint a [log4j](log4j.html) csak nem olyan fullos. Ugyhogy megsem...

Szóval:

*   [log4j](log4j.html)
*   [slf4j](slf4j.html)
*   Java loging api
*   [commons-logging](commons-logging.html)
*   [logback](logback.html) aka. log4j NG



Tenyesznek egyeb logging apik a neten:
*   Ezt a marhat verjetek agyon: https://simple-log.dev.java.net/
*   [Avalon](avalon.html) logger, ez a jelenleg aktualis [fop](FOP.html) egyik dependencyje, agyon kene csapni oket erte...
