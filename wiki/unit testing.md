---
creationDate: 1164881362053 
author: kocka 
contentAuthor: kocka 
title: unit testing 
contentUpdateDate: 1164881951744 
name: unit testing 
layout: wiki 
date: 1164881951744 
creator: kocka 
---
Olyan [test](test.html) ami egy bizonyos komponenst tesztel. Nyilvan a komponenssel szemben kell hogy legyen valami elvarasunk. ([COP](COP.html))

Frekventaltan visszatero eldontendo kerdes:

# Teszteljunk-e privat metodusokat?

Sokan csinaljak azt hogy a private nem lesz private csak package protected, es a teszteket ugyanabba a package strukturaba teszik mint a tesztelendo osztalyt, igy meg ha kulon forrasfaban is van, az [eclipse](Eclipse.html) (na, mar tool dependency-nel tartunk, figyeltek) le fogja tudni futtatni. 

A masik iranyzat azt mondja hogy private metodusokat nem tesztelunk. Csak a publikus, barki altal hasznalhato interface-re irunk tesztet, ha az atmegy, akkor a komponens megfelel az elvarasoknak.

# Nem visz el tul sok idot a tesztek irasa?

Maganvelemeny ([kocka](kocka.html)): neha igen, de tobbnyire [COP](COP.html) eseten jobban jar az ember ha minden komponenst ki tud fejleszteni es letesztelni egyenkent, majd a vegen integral, igy a hibak tenyleg azokban a komponensekben jelentkeznek, amelyikekben keletkeznek. Igy a tesztek fejlesztesenek ideje N-nel megszorozva kivonodik a debugolasra szant idobol.


