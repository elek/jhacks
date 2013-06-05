---
creationDate: 1106513476570 
author: kocka 
contentAuthor: kocka 
title: Adatbazis 
contentUpdateDate: 1115364476095 
name: Adatbazis 
layout: wiki 
date: 1115364476095 
creator: kocka 
---
[zsoltk](zsoltk.html) billentyuzetebol:

Most latom csak, hogy DB snip nincs. Pedig az egyik legalapvetobb eszkoz amit minden [J2EE](j2ee.html) fejleszto es [Corporate Developer](Corporate%20Developer.html) hasznal.<br/> Arra szolgal, hogy az alkalmazast hasznalo userek a midenfele adataikat meg tudjak orizni. Egyszoval mindenfele [OR Mapping](OR%20Mapping.html) dolog csak arrol szol, hogy az adatbazisban tarolt adatokat valahogy az alkalmazashoz jutassuk.<br/>

Tobb nagy alfaja van, de mara a nagy reszuk kihalt es ketto maradt: Relacios es Objektum Relacios. Kicsit kesobb kaptok majd leirast mindekettorol, de aki nagyon ezzel akar foglalkozni az vegye meg az [Adatbázisrendszerek - Alapvetés](http://www.panem.hu/a_konyv.php?konyv=64) cimu konyvet. Ott szepen leirnak mindent amit jo ha tud az ember.<br/>

Latszolag nem fontosabb resz egy alkalmazasban mint az osszes tobbi, de valojaban a legfontosabb. A szopasok 80 szazaleka abbol adodik, hogy az adatbazis tervet keszito embereknek nem sikerult megfeleloen interpretalni a [domain](domain.html)-t es valami elkefelt dizajn-t dobtak ossze. Amit kesobb maguk sem ismernek be, de idovel az egyszeru fejlesztuk karomkodasa es elegedetlensege egyre hangosabb lesz.;) _(Forradalmat ne varjon senki, ez nem az a topic)_<br/>

Amit meg erdemes tudni a mai vilagban es ezt a legutobbi projecten tanultam meg igazan: __mindegy mi van, az adatbazis design-nak jonak KELL lennie.__

Es akkor jojjenek a kapcsolodo snip-ek:<br/>
Relacios adatbazisok:
1. [MySQL](MySQL.html) Gyors, sokan hansznaljak, ennek ellenere nem a legjobb.
1. [Oracle](Oracle.html) Lassu, meg tobben hasznaljak es pont ezert nem a legjobb.
1. [Pointbase](Missing.html) Java alapu DB. Szep, okos, gyors, keveset fogyaszt es minden appszerver melle csomagoljak.
1. [HSQL](HSQL.html) Masik Java alapu DB. Lasd fent, csak eppen nem csomagoljak.
1. [Progress](Progress.html) Regi darab. Regi idokbol. Ennek ellenere nagyon jo kis darab. Csak ne akard JDBC-n keresztul hasznalni:)
1. [MAXDB](MAXDB.html) [Kocka](kocka.html)?
1. [MSSQL](MSSQL.html) Mert a [Microsoft](Microsoft.html) ilyet is gyart:)

Objektum Relacios adatbazisok:
1. [PostgreSQL](PostgreSQL.html) Az egyetlen:) [Kocka](kocka.html)?<br/>

Na hirtelen ennyit az adatbazisokrol. Egyebkent a snipet azert csinaltam, hogy betehessek egy linket: [Azzurri Clay, Database Modeling in Eclipse](http://www.azzurri.jp/en/software/clay/index.jsp). Egyetlen hibaja, hogy nem free.

Valojaban az [RDBMS](RDBMS.html) snip elobb volt, de ezen tobb a szoveg. Mindenesetre az [adatbazis](Adatbazis.html) snippen kellene lennie, amjd kesobb letorlom atpakolom a tartalmat.


Erdetileg ez a snipsnap-index/Adatbazis snipp volt. Napalmmal dobalok mindenkit aki ezutan a [snipsnap-index](snipsnap-index.html) ala snippet hoz letre.

Lasd meg: [RDBMS](RDBMS.html)
