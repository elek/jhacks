---
creationDate: 1158831682367 
author: kocka 
contentAuthor: kocka 
title: Laszlo/laszlo webapp build 
contentUpdateDate: 1182763156436 
name: Laszlolaszlo webapp build 
layout: wiki 
date: 1182763156436 
creator: kocka 
---
Nehany esetben kicsit azert izgis ez a [laszlo](../Laszlo.html), mert nem egeszen ugy kell ala fejleszteni mint egy sima [webapp](../webapp.html), meg ha egy teljesen sima [webapp](../webapp.html) is lesz belole. Na jo, flash-es. Kit erdekel :) Szoval kicsit okositani kell a [build](../build.html) processt.

Szoval eredetileg ugy kell alkalmazast deployolni laszlo ala hogy bemasolgatod a classfileokat, a [laszlo/lzx](../laszlo/LZX.html) fileokat, megpatcheled a web.xml-t, aztan ujrastartolod a kontextet es lass csodat.

Hat ez eleg manualis, de van ennel nemileg emberibb megoldas.

*   irsz egy [ant](../ant.html) scriptet. Nem irom meg helyetted, hajra :)
*   egyszeruen [maven/maven2](../maven/maven2.html)-vel, beteszel egy dependency-t az openlaszlo war file-ra, meg azt jelezned kell hogy ez egy __runtime__ dependency. a war plugin ki fogja neked csomagolni az openlaszlo war file-t, belerakja a sajat cuccodat es csinal belole egy uj war filet, ez mar futtathato 'mvn [jetty](../jetty.html):run' paranccsal, vagy deployolhato, amit akarsz.
