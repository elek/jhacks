---
creationDate: 1202766696656 
author: karenin 
contentAuthor: karenin 
title: SDO 
contentUpdateDate: 1202769655851 
name: SDO 
layout: wiki 
date: 1202769655851 
creator: kocka 
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
