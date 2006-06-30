---
creationDate        : 2006-06-30 11:19:02 +0200 
author              : kocka 
title               : classloader 
name                : classloader 
layout              : wiki 
path                : classloader 
date                : 2006-06-30 11:19:02 +0200 
version             : 1 
creator             : kocka 
---
A [java.lang.ClassLoader](http://docs.oracle.com/javase/7/docs/api/java/lang/ClassLoader.html) es az o dicso leszarmayottai.

Egy teljesen ujszeru koncepcio volt a [java](java.html)ban mar a legelejen, mondhatni core java feature. Mindenesetre a VM a classloader hierarchiat hasznalja amikor egy osztalyt be kell tolteni.

A legjobb, hogy ebbol nyilvan nagyon sokfele lehet, tolthetsz be osztalyokat adatbazisbol, filerendszerrol, halozatrol, mazohistak billentyuzetrol is akar :) Ami meg ennel is uberebb, az az hogy a classloadereid viselkedeset megvalotoztathatod es konfiguralhatod magad.

Erdekes peldaul a [classworlds](Missing.html) es a [loom](loom.html) sajat belso kis classloader konfiguracios rendszere, valamint a [POMstrap](POMstrap.html) is erdekes otlet. Szoval ezzel az egesszel el lehet tolteni par utolag haszontalannak minositett percet, orat, napot...
