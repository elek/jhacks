---
creationDate        : 2005-02-16 15:41:19 +0100 
author              : kocka 
title               : C 
name                : C 
layout              : wiki 
path                : C 
date                : 2005-06-26 15:23:46 +0200 
version             : 6 
creator             : kocka 
---
Egy meglehetosen regi, proceduralis nyelv. Nevet az A-rol es a B-rol kapta :) Elsosorban [operacios rendszer](Operacios%20rendszer.html)ekhez, vagy rendszerkozeli funkcionalitashoz, beagyazott cuccokhoz.

A Portolhatosag nem eppen a legfobb erenye, de megoldhato (posix).

__C-ben is lehet objektum orientalt ([OOP](oop.html)) modszerekkel dolgozni__ Csak nem szokas.

A C egy valamennyire modernizalt valtozata a C++, ez [OOP](oop.html) es tobbnyire a [java](java.html)val szoktak osszehasonlitani, viszont inkab csak egy hack a C nyelven. Nincs hozza szabvanyos felulet, virtualis gep, [GC](GC.html), exceptionok vannak, de igazabol csak olyan amit te csinalsz bele, szoval a szabvanytalansag egy java programozo szamara kisse fapados nyelv erzeset kelti. Nagyon nem szoktak a C++-t szeretni a szerver projectek fejlesztoi, eleg zuros osszeintegralni akar sajatmagaval is. Elonye hogy [OOP](oop.html) es csak kicsit lassabb mint a [C](C.html), meg egy tucat syntax sugar :)

Ami igazan nagyon tud fajni a C nyelvben az a [build](build.html) rendszerek. Egyszeru esetekre rettenetesen konnyu makefile-t irni, de ez kb a 'hello world' kategoriaig igaz, aztan jonnek a csunya dolgok. A legbaratsagosabbnak [GNU](GNU.html) fejlesztokornyezetet nevehetjuk, szerencsere eleg elterjedt is, de messze nem osszehasonlithato egy olyannal hogy '[maven](maven.html) dist' peldaul vagy '[ant](ant.html) ize'. Amellett ott van a sok izgalmas build kornyezet mint pl a [SAPDB](SAPDB.html) cucca vagy mas closed source multu dolog.

# Eszkozok

C-hez is vannak [IDE](IDE.html)k ugyanugy mint javahoz, bar ezek inkab platformspecifikusak, [linux](Linux.html)on nagyon ql a kdevelop es az anjuta, szemelyes kedvencem viszont a [vim](VIM.html)+bash.

[Eclipse](Eclipse.html) hez C plugin a [Eclipse/Plug-in/CDT](Eclipse/Plug-in/CDT.html). 

Kicsit faj veluk a debugolas, sehogy sem olyan kiraly mint [java](java.html)ban.

Lasd meg: [JNI](JNI.html)
