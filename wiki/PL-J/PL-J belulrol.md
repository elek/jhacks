---
creationDate        : 2005-01-02 23:33:14 +0100 
author              : kocka 
title               : PL-J/PL-J belulrol 
name                : PL-J/PL-J belulrol 
layout              : wiki 
path                : PL-J/PL-J belulrol 
date                : 2005-01-03 00:00:43 +0100 
version             : 8 
creator             : kocka 
---
_Most meglatjatok milyen rettenetes abraka lehet rajzolni gimppel egy kis hozzaertes es igenyesseg nelkul :)_

A [PostgreSQL](../PostgreSQL.html) koruli java tarolt eljaras rendszerek eseteben mindig kerdes volt a kommunikacio megvalositasa. A problema abbol adodik hogy a PostgreSQL nem threadel, mig a Java ha kell ha nem threadeket indit, ez a ketto nem jatszik szepen egyut, igy a [JNI](../JNI.html) megvalositast alaposan korbe kell falazni, viszont ha kulon processzekben fut a java es a postgres, akkor elofordulhat hogy a processzek kozti kommunikacio lesz a bottleneck, de ha nem az akkor az orokonos processzvaltasok.

![image](http://hackers.forgeahead.hu/space/PL-J/PL-J+belulrol/plj-db-interaction.gif)

Szoval ezt vegiggondolva, megis melyik uton induljak, akkor igy dontottem: socketelek, de a [JNI](../JNI.html) is hagyok helyet. Ebbol jott letre a kommunikacios csatorna api ami kisse low level, es nem igazan konnyu hasznalni de ez mindegy mert ugyis csak nekem kell, es lehetove teszi hogy masfele implementaciokat helyettesitsunk be. Ezzel a designnal, kb ugy nez ki mint egy apache [httpd](../httpd.html) -> [mod_jk](../mod_jk.html) -> [tomcat](../tomcat.html), csak mindez adatbazis layeren.


Szoval a PL-J [IoC](../ioc.html) elkepzeleseken alapszik, kis tucat komponensbol epul fel, amit termeszetesen akar at is lehet irni ha valaki annyira jol nyomja :)<br/>
Egy komponens egy adott feladatkort tolt, tobbnyire eleg aprokat, pl a log4j rendszer bekonfiguralasa, ilyesmi. A legfobb komponens tipusok:

*   __channel__, ami a kommunikaciot valositja meg, 
*   __typemapper__, ami RDBMS tipusokat tud mappelni Java osztalyokka es vissza
*   __executor__, a UDF/trigger hivasok futtatasa.

![image](http://hackers.forgeahead.hu/space/PL-J/PL-J+belulrol/plj-components-overview.gif)

Persze mindegyik konkret megvalositasa egyeb komponsnsek hasznalatat teszi szuksegesse vagy celszeruve, igy szulettek olyan kulon szerviz komponensek, mint:

*   __JDBC konfiguracio szolgaltatas__, igy az alkalmazasodban tudod konfiguralni a JDBC driver viselkedeset. (Kicsit sokfele opcio van...)
*   [Log4j](../log4j.html) inicializalo szolgaltatas.
*   stb

A [Loom](../loom.html) alkalmazasszerver sok finom szolgaltatast nyujt: [JMX](../JMX.html), hot deploy, az alkalmazas tobb alkalmazassal egy VM-ben tud futni, stb.

![image](http://hackers.forgeahead.hu/space/PL-J/PL-J+belulrol/plj-in-loom.gif)


(folytkov, rettegj retek!)
