---
creationDate        : 2004-08-04 12:43:45 +0200 
author              : admin 
title               : Data Access Object 
name                : DAO 
layout              : wiki 
path                : DAO 
date                : 2006-03-26 01:42:36 +0100 
version             : 1 
creator             : zsoltk 
---
Amolyan adateleresi reteg OOP modra. Jellemzoen arra szolgal, hogy a relacios adatbazis tulajdonsagait, kezeleset elrejtsuk a felhasznalo elol es egy OOP-ban jobban (nem biztos hogy egyszerubben) hasznalhato nezetet adjuk az adatbazis strukturanak. (lasd meg: [OR Mapping](OR%20Mapping.html))

Jellemzoi:

*   Absztrak osztalyok, interfacek melyek csak a funkciokat irjak le.
*   A funkciok az adatbazisobjektumok irasa, olvasasa, modositasa.
*   Minden adattablanak egy objektum felel meg.
*   A mapping nem automatikusan, hanem kezzel tortenik.
*   Tobbfele adatbazishoz irhato implementacio.

Altalaban egyszeru, konnyen olvashato, atlathato strukturat eredmenyez, ehhez viszont az kell, hogy maga az adatbazis ne legyen tul bonyolult. Hatranya, hogy mindent kezzel kell megirni, bar erre is van megoldas: [Mr. Persister](Mr.%20Persister.html)

A temaban egy eleg hasznos cikk: [http://www-106.ibm.com/developerworks/java/library/j-dao/](http://www-106.ibm.com/developerworks/java/library/j-dao/)
