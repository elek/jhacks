---
creationDate: 1121784996035 
author: karenin 
contentAuthor: karenin 
title: Simple Api for XML 
contentUpdateDate: 1181819463923 
name: sax 
layout: wiki 
date: 1181819463923 
creator: kocka 
---
( pont ugy kell kimondani mint azt hogy 'sucks', nem minden ok nelkul :) )

Egy api ami benne van a [jdk](Missing.html)-ban mar jo ideje es akkor celszeru hasznalni ha nagyon nagy [XML](XML.html) allomanyokat akarsz feldolgozni. Nem hoz letre egy reprezentacios modellt mint a [DOM](dom.html), hanem eventeket kuldozget a listenerednek. Igy megtakarit egy csomo memoriat, meg dolgozhatsz vele egy csomot. 

Tipikus push parser, azaz ha elkezd parsolni, akkor nyomja bele az eventeket a listenerednek, amig csak tart a fajl.

Hasonloan hatekony, csak pull parser megoldas a [StAX](StAX.html)
