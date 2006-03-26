---
creationDate        : 2005-04-07 16:21:48 +0200 
author              : admin 
title               : 2 Phase Commit 
name                : 2PC 
layout              : wiki 
path                : 2PC 
date                : 2006-03-26 01:42:33 +0100 
version             : 1 
creator             : kocka 
---
Egy regi technologia, az eloszotott tranzakciok nagyobb biztonsagaert talaltak ki. Elso fazisban a tranzakcioban reszt vevo eroforrasokat a tranzakcio vezerlo felszolitja szavazasra, ekkor a minden eroforras kezelo leellenorzi a sajat konzisztenciajat, majd ha minden eroforras kezelo igennel szavazott, akkor commitot kuld nekik a tranzakcio vezerlo. Ekkor mindegyiknek vegre kell hajtani a modositast.

Nyilvan konnyen lehet olyan lehetoseget talani amikor a 2PC kiakadna, semmi sem atombiztos, de be kell latni hogy eleg kicsire csokkenti a valoszinuseget.

Lasd: [JTA](JTA.html), [JTS](JTS.html)
