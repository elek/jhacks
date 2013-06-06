---
creationDate        : 2008-02-11 22:51:36 +0100 
author              : karenin 
title               : SDO 
name                : SDO 
layout              : wiki 
path                : SDO 
date                : 2008-02-11 23:40:55 +0100 
version             : 3 
creator             : kocka 
---
Service Data Objects

Az [SCA](SCA.html) párja, adatstruktúrák tárolására nyelv és platformfüggetlen környezetbe.

Képzeljünk el egy nagy DOM fát. A levelek mind namespace által meghatározottak. De az egész dolog XML független. Vannak hozzá ügyes átalakítók, amik ki tudják szerializálni a fát akár adatbázisba, akár XML-be, akárhová.

A fa egyes szintek elérésének is különböző interface-ük van. Lehetnek Pojo-k, de Hashmap jellegű kevésbé típusos API-n keresztül is lekérhetőek az értékek.

Plusz még egy két szolgáltatás, pl. verziózás.

Valami ilyen emlékem maradt belőle, de majd kijavítja, aki többet használta.

Pl. az [Apache](apache.html) [Tuscany](http://incubator.apache.org/tuscany/)-ja tudja a dolgot.


Egyenlore csak linkek: [IBM](http://www-106.ibm.com/developerworks/java/library/j-commonj-sdowmt/), 
[BEA](http://dev2dev.bea.com/technologies/commonj/sdo/index.jsp)
