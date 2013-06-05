---
creationDate: 1091611672782 
author: kocka 
contentAuthor: kocka 
title: Object Relation Mapping 
contentUpdateDate: 1212835470424 
name: OR Mapping 
layout: wiki 
date: 1212835470424 
creator: zsoltk 
---
De mivel ez nem teljesen ertheto, ezert egy kicsit bovebben: Relacios adatbazis tablainak mappelese Objektum orientalt kornyezetbe.

Hogy mirol is van szo bovebben?

Ne arra gondolj, hogy az adatbazis tablaiban levo mezok ertekeibol kepzunk objektumokat, hanem arra, hogy magukbol az adatbazis tablakbol. Azoknak minden tulajdonsagaval, kapcsolataval egyutt.

Ilyen mondon, letrehozva egy kvazi Objektumrelacios adatbazist. Azert kvazi, mert maga az adatbazis meg mindig relacios, mi viszont objektumrelaciosnak latjuk.

Nagy elonye a hagyomanyos megkozelitessel szemben, hogy a programjainkban nem kell kulonosebben foglalkozni az adatbazis felepitesevel. Nem kell SQL muveleteket irogatnunk. Nem kell kulon foglalkoznunk a tablak kapcsolataival. Egyszoval nagyban meg tudja konnyiteni az eletunket.

A temaban egy atfogo elmeleti munka: http://www.chimu.com/publications/objectRelational/index.html

Valamint a kulonbozo libek és apik:

*   Egyik es legfontosabb az [EJB](EJB.html), azon belul pedig az [Entity Bean](Missing.html).
*   Masik, amit sokan szeretnek: [Hibernate](Hibernate.html)
*   Ugyanaz, csak egy kicsit mas felfogasban: [Mr. Persister](Mr.%20Persister.html)
*   Egy Hibernate-hez hasonlo dolog, csak nem annyira eros: [Torque](Torque.html)
*   Az [ejb3](EJB3.html)-al bevezetett Java Persistence Api([JPA](JPA.html)), ami alá több megoldást is be lehet rakni. 
