---
creationDate        : 2005-03-29 09:57:06 +0200 
author              : kocka 
title               : PostgreSQL/Architektura 
name                : PostgreSQL/Architektura 
layout              : wiki 
path                : PostgreSQL/Architektura 
date                : 2006-02-14 23:13:59 +0100 
version             : 2 
creator             : kocka 
---
A [PostgreSQL](../PostgreSQL.html) eleg egyszeru, fork-os rendszer, azaz minden klens egy kulon processzt kap, ami kiszolgalja, a processzek osztott adataikat (lock, cache, stb) egy osztott memoria szegmensben tartjak. Az egy processz egy szalu, azaz egyetlen szalon szolgalja ki a felhasznalot. (azert valamit dobna rajta a tobbszalusag de mindig lehurrognak amikor ilyeneket mondok :) )

Nem sokat bonyolit a rendszeren a bgwriter processz sem, ez a hatterben futo adatfile iro.

Az egyszeru architektura persze helyenkent visszaut. Pl a [blob](../blob.html)okat egy pg_largeobject tablaban tartja, az osszeset. A bokkeno itt az, hogy nem is torli le onnan, se akkor ha a sort torlod, se akkor ha az egesz tablat droppolod. Implicit torolni kell, vagy nagy importok eseten erdemes ujra letrehozni az adatbazist.
