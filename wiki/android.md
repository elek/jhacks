---
creationDate        : 2007-11-15 22:39:44 +0100 
author              : karenin 
title               : Google Android 
name                : android 
layout              : wiki 
path                : android 
date                : 2007-11-15 23:58:59 +0100 
version             : 2 
creator             : kocka 
---
[http://code.google.com/android/](http://code.google.com/android/)

Szabad mobil platform fejlesztés, az ipar elég nagy támogatásával. A programokat Java-ban kell írni hozzá, de nem hagyományos byte code-ra fordítja, és egy saját VM futtatja a programokat. (Habár a common lib hagyományos JAR-ban van mellette.)

A fő varázslat benne az Intent osztály köré épülő hívás struktúra. Gyakorlatilag több paraméter alapján handler szerű dolgokat lehet regisztrálni, és ezekkel lehet a modulokat egymáshoz kapcsolni. Így elvileg minden részét (akár az adressbook-ot, vagy a főoldalt) ki lehet cserélni az alap alkalmazásnak, illetve hozzá lehet majd kapcsolódni bármilyen eseményhez (pl. SMS érkezése).

Hpsszú távon az SDK (tehát a VM is) Open Source lesz, de source-ból az első release-t csak az első hardware-ek megérkezése után adják ki.

Vannak akik kétkedéssel fogadják, de Java fejlesztők számára mindenképpen ultimate mobilnak ígérkeznek az androidok.

*   [Ide](IDE.html) support: [eclipse](Eclipse.html) plugin 
*   [Linux](Linux.html) kernelen fut
*   Hardware egyelőre nincs hozzá, csak az SDK-hoz mellékelt emulátoron lehet játszani. (Bár a hivatalos reklám videókon látszik, hogy a Guglinak már vannak teszthardverei)


