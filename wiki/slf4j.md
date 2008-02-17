---
creationDate        : 2008-02-17 22:26:46 +0100 
author              : karenin 
title               : slf4j 
name                : slf4j 
layout              : wiki 
path                : slf4j 
date                : 2008-02-17 22:26:46 +0100 
version             : 1 
creator             : karenin 
---
Simple Logging Facade for Java 
[http://www.slf4j.org/](http://www.slf4j.org/)

Ahogy a neve is mutatja, csak egyfajta közös felületet nyújt a meglévő [logging](Logging.html) megoldásokra. Valahogy úgy kell elképzelni, mint az összes jó loggoló framework legnagyobb közös osztóját, azaz csak az a nagyon alap van benne, ami mindegyikben. 

Cserébe azt a kellemes illúziót biztosítja, hogy nagyon függetlenek vagyunk a logging implementációktól. Gyakorlatban én úgy szoktam vele találkozni, hogy letöltök valami cuccot, amiben a függőségek között csak a slf4j-api van, azzal a felkiáltással, hogy majd én töltsem le akárhonnan azt az implementációt amit szeretnék.

(Ez egyébként [log4j](log4j.html)-nél pl. egy csatolót és magát a log4j-t is jelenti, de pl. a [logback](logback.html)-ben már be van építve az slf4j támogatás.)

ps: Aki nagyon látja az értelmét, az kérem győzzön meg.
