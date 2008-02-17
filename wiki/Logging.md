---
creationDate        : 2005-07-13 11:12:24 +0200 
author              : karenin 
title               : Logging 
name                : Logging 
layout              : wiki 
path                : Logging 
date                : 2008-02-17 22:18:58 +0100 
version             : 4 
creator             : kocka 
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

*   Ezt a marhat verjetek agyon: [https://simple-log.dev.java.net/](https://simple-log.dev.java.net/)
*   [Avalon](avalon.html) logger, ez a jelenleg aktualis [fop](FOP.html) egyik dependencyje, agyon kene csapni oket erte...
