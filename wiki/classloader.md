---
creationDate: 1151659142703 
author: kocka 
contentAuthor: kocka 
title: classloader 
contentUpdateDate: 1151659142703 
name: classloader 
layout: wiki 
date: 1151659142703 
creator: kocka 
---
A  es az o dicso leszarmayottai.

Egy teljesen ujszeru koncepcio volt a [java](java.html)ban mar a legelejen, mondhatni core java feature. Mindenesetre a VM a classloader hierarchiat hasznalja amikor egy osztalyt be kell tolteni.

A legjobb, hogy ebbol nyilvan nagyon sokfele lehet, tolthetsz be osztalyokat adatbazisbol, filerendszerrol, halozatrol, mazohistak billentyuzetrol is akar :) Ami meg ennel is uberebb, az az hogy a classloadereid viselkedeset megvalotoztathatod es konfiguralhatod magad.

Erdekes peldaul a [classworlds](Missing.html) es a [loom](loom.html) sajat belso kis classloader konfiguracios rendszere, valamint a [POMstrap](POMstrap.html) is erdekes otlet. Szoval ezzel az egesszel el lehet tolteni par utolag haszontalannak minositett percet, orat, napot...
