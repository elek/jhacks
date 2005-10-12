---
creationDate        : 2005-10-12 09:57:56 +0200 
author              : renszarv 
title               : escape analysis 
name                : escape analysis 
layout              : wiki 
path                : escape analysis 
date                : 2005-10-12 11:32:56 +0200 
version             : 2 
creator             : kocka 
---
[kocka](kocka.html) szerint:~~Ez valami olyasmi hogy csekkolja hogy a programod hogy er el objektumokat, es azt felhasznalja ahhoz hogy erosebben parhuzamosithato legyen.


Vagy valami ilyesmi :)~~

Valóságban ez azt jelenti, hogy vizsgálja, hogy az objektumokat amiket létrehozol egy metódusban, azt felhasználod e a metóduson kivül is. Mert ha nem, akkor csak a [stack](Missing.html)en hozza létre számára a helyet, nem a globális [heap](Missing.html)en. Ez jelentősen gyorsabbá teheti a dolgokat.
