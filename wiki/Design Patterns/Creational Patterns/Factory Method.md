---
creationDate        : 2007-09-27 15:05:53 +0200 
author              : karenin 
title               : Design Patterns/Creational Patterns/Factory Method 
name                : Design Patterns/Creational Patterns/Factory Method 
layout              : wiki 
path                : Design Patterns/Creational Patterns/Factory Method 
date                : 2007-09-27 15:05:53 +0200 
version             : 1 
creator             : karenin 
---
A lényeg az, hogy ne interface-re gondoljunk, hanem abstract osztályra.

Mondjuk van egy Jármű absztrakt osztályunk, aminek van createKerék() és cserélKerék() függvénye. Az előbbi absztrakt, hiszen a Szekérben más fajta kereket kreálunk, mint mondjuka Kocsi-ban. Viszont a cserélKerék egész konkrét, neki mindegy, hogy melyik kerék van, azt null-ra állítja, és aztán kicseréli azzal, hogy meghívja a createKerék() metódust, ami egy gyerek osztályban lesz implementálva. Tehát a factory method egy konkrét gyerek osztályban van implementálva, de már az absztrakt ős használja a gyümölcsét (nyilván itt is interface-en keresztül).

Na, ez nem biztos, hogy érthető lett, pedig valami ilyesmiről van szól.
