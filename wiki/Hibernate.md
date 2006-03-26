---
creationDate        : 2004-08-04 11:32:34 +0200 
author              : admin 
title               : Hibernate 
name                : Hibernate 
layout              : wiki 
path                : Hibernate 
date                : 2006-03-26 01:42:40 +0100 
version             : 1 
creator             : zsoltk 
---
Talan az egyik legerosebb [OR Mapping](OR%20Mapping.html) cucc. Nagyon sok mindent tud, kelloen bonyolult, szepen idomithato, erdekes koncepciok. Bovebbet nem tudok, mivel magam meg nem hasznaltam, csak a specifikaciojat olvastam vegig.

A hibernate nem nyilt szabvany alapu cucc, hanem egyeszeruen csak egy API, de a gyakorlati feladatokat sokkal jobban kozeliti. Talan pont ezert. Mivel [LGPL](LGPL.html)es, szabadon felhasznalhato, azaz terjedhet ezerrel :)
Valojaban egy reteg a [JDBC](JDBC.html) api felett, nyilvan igy nem tudja a leheto legeffektivebben ellatni a feladatait, de tobbnyire ellatja. Pl insert teljesitmenyen lehetne valamit hangolni mert kozel sem optimalis, de ez igazabol senkit sem zavar.

[Webapp](webapp.html)okban nagyon jo moka peldaul az, hogy egy egeszen egyszeru actionnal felhozol egy bean-t az adatbazisbol, atadod a view layernek, es a view a kapcsolatait is borzaszto egyszeruen meg tudja jelniteni, es az actionnak nem kellett feltetlenul tudnia a view miket akar majd megjeleniteni. Szoval sokat egyszerusit az ember eleten.

Az [EJB3](EJB3.html) specifikacio nagyon kedvez a hibernate-nek.

link: [http://hibernate.org/](http://hibernate.org/)
