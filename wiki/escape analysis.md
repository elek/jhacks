---
creationDate: 1129103876515 
author: renszarv 
contentAuthor: renszarv 
title: escape analysis 
contentUpdateDate: 1129109576457 
name: escape analysis 
layout: wiki 
date: 1129109576457 
creator: kocka 
---
[kocka](kocka.html) szerint:~~Ez valami olyasmi hogy csekkolja hogy a programod hogy er el objektumokat, es azt felhasznalja ahhoz hogy erosebben parhuzamosithato legyen.


Vagy valami ilyesmi :)~~

Valóságban ez azt jelenti, hogy vizsgálja, hogy az objektumokat amiket létrehozol egy metódusban, azt felhasználod e a metóduson kivül is. Mert ha nem, akkor csak a [stack](Missing.html)en hozza létre számára a helyet, nem a globális [heap](Missing.html)en. Ez jelentősen gyorsabbá teheti a dolgokat.
