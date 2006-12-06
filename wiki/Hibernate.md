---
creationDate        : 2004-08-04 11:32:34 +0200 
author              : kocka 
title               : Hibernate 
name                : Hibernate 
layout              : wiki 
path                : Hibernate 
date                : 2006-12-06 13:25:10 +0100 
version             : 6 
creator             : zsoltk 
---
[http://hibernate.org/](http://hibernate.org/)

Talan az egyik legerosebb [open source](Open%20Source.html) [OR Mapping](OR%20Mapping.html) cucc ([LGPL](LGPL.html)). Implementalja a javax.persistence apit, azaz a 3.2 releasetol most mar teljesen szabvanyos feluleten keresztul is hasznalhato.

Valojaban egy reteg a [JDBC](JDBC.html) api felett, nyilvan igy nem tudja a leheto legeffektivebben ellatni a feladatait, de tobbnyire ellatja. Pl insert teljesitmenyen lehetne valamit hangolni mert kozel sem optimalis, de ez igazabol senkit sem zavar.

[Webapp](webapp.html)okban nagyon jo moka peldaul az, hogy egy egeszen egyszeru actionnal felhozol egy bean-t az adatbazisbol, atadod a view layernek, es a view a kapcsolatait is borzaszto egyszeruen meg tudja jelniteni, es az actionnak nem kellett feltetlenul tudnia a view miket akar majd megjeleniteni. Szoval sokat egyszerusit az ember eleten.

Az [EJB3](EJB3.html) specifikacio nagyon kedvez a hibernate-nek.

Lasd meg: [or mapping](OR%20Mapping.html), [persistence](persistence.html)


