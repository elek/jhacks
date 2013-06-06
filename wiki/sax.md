---
creationDate        : 2005-07-19 16:56:36 +0200 
author              : karenin 
title               : Simple Api for XML 
name                : sax 
layout              : wiki 
path                : sax 
date                : 2007-06-14 13:11:03 +0200 
version             : 2 
creator             : kocka 
---
( pont ugy kell kimondani mint azt hogy 'sucks', nem minden ok nelkul :) )

Egy api ami benne van a [jdk](Missing.html)-ban mar jo ideje es akkor celszeru hasznalni ha nagyon nagy [XML](XML.html) allomanyokat akarsz feldolgozni. Nem hoz letre egy reprezentacios modellt mint a [DOM](dom.html), hanem eventeket kuldozget a listenerednek. Igy megtakarit egy csomo memoriat, meg dolgozhatsz vele egy csomot. 

Tipikus push parser, azaz ha elkezd parsolni, akkor nyomja bele az eventeket a listenerednek, amig csak tart a fajl.

Hasonloan hatekony, csak pull parser megoldas a [StAX](StAX.html)
