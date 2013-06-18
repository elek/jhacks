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
tags:
   - mobil
---
[http://code.google.com/android/](http://code.google.com/android/)

Szabad mobil platform fejlesztés, az ipar elég nagy támogatásával. A programokat Java-ban kell írni hozzá, de nem hagyományos byte code-ra fordítja, és egy saját VM futtatja a programokat (Dalvik VM).

Az hogy mennyire szabad vita tárgya. [Open source](Open source.html), tehát még így is jobb mint bármi más, de a Google azért elég erős kontrolt gyakorol fölötte. Például a fejlesztés nem publikus, csak a nagy verziók megjelenése után publikálják a kódot.

Mindenesetre az android szép lassan ledarálja az okostelefon piacot és egyelőre nem úgy tűnik, hogy bárki is meg tudja állítani.

A programozása Java-ban van (de van lehetőség natív kódok futtatására is), még ha az APIja néha kicsit gány. A képernyők egy speciális Inter process communication szerű dolgon keresztül beszélgetnek, ami kicsit bonyolítja a fejlesztést, de cserébe jól kezelhető az, amikor erőforrás szűke miatt az oprendszer takarít. A másik, ami jól ki van benne találva, hogy az egyes alkalmazások hogy tudják egymás funkcióit használni vagy kiterjeszteni. Ezért a fő képernyőtől kezdve szinte minden felülírható benne.

*   [Ide](IDE.html) support: Gyakorlatilag mára már mindenki támogatja. A hivatalos IDE eddig az [eclipse](Eclipse.html)-re épülg pluginek formájában, de újabban úgy tűnik átnyergelnek [IDEA](idea.html)-ra.
*   [Linux](Linux.html) kernelen fut



