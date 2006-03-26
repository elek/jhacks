---
creationDate        : 2005-01-18 09:20:57 +0100 
author              : admin 
title               : pljava 
name                : pljava 
layout              : wiki 
path                : pljava 
date                : 2006-03-26 01:48:37 +0100 
version             : 1 
creator             : kocka 
---
[http://gborg.postgresql.org/projects/pljava/](http://gborg.postgresql.org/projects/pljava/)

Egy java tarolt eljaras nyelv [PostgreSQL](PostgreSQL.html)-re, [JNI](JNI.html) megoldassal.

Szal nezzuk csak. Miben all a [PL-J](PL-J.html) es a [PLJava](pljava.html) ellentete: 

*   A PLJava alapbol JNI-n keresztul hiv java metodusokat
*   A [PostgreSQL](PostgreSQL.html) forkos allat
*   Minden processzhez tehat sajat JVM-et kell letrehozni.
*   Ez jelentos ido az elso hivasnal, de utanna rendkivul gyorsan fut a VM.
*   Viszont valami eszement mennyisegu memoriat emeszt fel. Az adatbazis processzek memoriajahoz kepest nagyon nagyok lesznek a JVM memoriafoglalasok.
*   Marpedig nekem azert kell sok memoria a DB szerver gepbe hogy az adatot keselje benne, ne a tucat JVM-et. 20 kapcsolat 60 MB-tal szamolva 1200 Mega, egy ekkora memoriaju geptol elvarnam hogy ne csak 20 kapcsolatot tudjon kiszolgalni.

Hol tud egyutmukodni a ket rendszer:<br/>
Nos lehet hogy valahol egyut fog mukodni a ket rendszer bizonyos darabjai (valoszinuleg a [PL-J/DevTools](PL-J/DevTools.html)), meg IRC-en is leszogeztuk hogy mivel a felhasznalokkal nem akarunk kitolni, egyutmukodunk egyes megoldasokban. Na ez azota ugy mukodik hogy az arc szerint nekem kene kovetni az utasitasait, szoval itt tartunk, meglepodnek ha tovabb tudnanak lepni :)

Na ezt jo lefikaztam :)
