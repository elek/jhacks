---
creationDate: 1112883708573 
author: kocka 
contentAuthor: kocka 
title: 2 Phase Commit 
contentUpdateDate: 1112883708573 
name: 2PC 
layout: wiki 
date: 1112883708573 
creator: kocka 
---
Egy regi technologia, az eloszotott tranzakciok nagyobb biztonsagaert talaltak ki. Elso fazisban a tranzakcioban reszt vevo eroforrasokat a tranzakcio vezerlo felszolitja szavazasra, ekkor a minden eroforras kezelo leellenorzi a sajat konzisztenciajat, majd ha minden eroforras kezelo igennel szavazott, akkor commitot kuld nekik a tranzakcio vezerlo. Ekkor mindegyiknek vegre kell hajtani a modositast.

Nyilvan konnyen lehet olyan lehetoseget talani amikor a 2PC kiakadna, semmi sem atombiztos, de be kell latni hogy eleg kicsire csokkenti a valoszinuseget.

Lasd: [JTA](JTA.html), [JTS](JTS.html)
