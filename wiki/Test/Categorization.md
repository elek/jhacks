---
creationDate        : 2006-08-01 17:03:03 +0200 
author              : kocka 
title               : Test/Categorization 
name                : Test/Categorization 
layout              : wiki 
path                : Test/Categorization 
date                : 2006-08-01 17:03:03 +0200 
version             : 1 
creator             : kocka 
---
A tortenet kicsit kavar, mert aki csak [pojo](../pojo.html)kat kodol, az neha meg van gyozodve rola hogy a tesztek cefet gyorsan lefutnak, minden platformon, ugyhogy kar is kategorizalni egy project tesztjeit, le lehet barmelyik buildben futtatni siman.

Hat a vilag sajnos nem ennyire idealis, pedig de szep is lenne.

Vannak ugyanis kulonbozo [platform](../Missing.html)fuggo szolgaltatasok amikre egy alkalmazas epul, peldaul [rdbms](../RDBMS.html) platform meg [alkalmazas szerver](../Alkalmazas%20Szerver.html) platform, amiket szinten tesztelni kell de nem lehet minden kornyezetben vegrehajtani a tesztet (pl ha nincs orakulum installalva), meg a tesztek is tobbfelek, szoval ha mas mod nincs ra, akkor kategorizacioval elvalaszthato hogy mikor melyik tesztnek kell lefutnia.

Ez egy viszonylag uj koncepcio, peldaul a [junit](../junit.html)ban is csak a 4.1-tol van kategorizacio, [IDE](../IDE.html) support ilyesmihez meg egyaltalan nincs.