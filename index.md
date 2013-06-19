---
layout: default
title: JHacks
---

# Mi ez?

A jhacks.hu a 2000-es évek közepén szerkesztett Java témájú wiki volt. A fő szerkesztője [Kocka](http://iwillworkforfood.blogspot.ch/) volt. A wiki lassan technikai okok (a SnipSnap wiki motort nem fejlesztették tovább) és hoszting okok miatt is eltűnt, azonban megmaradt egy legutolsó változat SnipSnap dump formátumban.

A wiki oldal bár elavult, de sok érdekes információt tartalmaz a Java ökoszisztéma 2000-es évek beli állapotáról (ki emlékszik még pl. a régi IoC konténerekre). Ezért a dumpból statikus oldalt genráltam, és feltettem ide a github pages alá. 

Kezdéshez kattints az [Oldalindex](List.html)re, (illetve van egy elég korlátozott korhű [kezdőlap](wiki/topics.html) is)

Az oldalak nagyrésze 2004 és 2008 között íródott, de migráció közben nem tudtam megállni, hogy néhány oldalba ne szerkesszek bele. Érdemes mindig a bal alsó sarokban megnézni ay utolsó módosítást mielőtt bármit készpénznek veszünk...

# Szerkesztés

Ahogy írtam első sorban archívumot akartam létrehozni, de ahogy nekem is kedvem támadt közben szerkeszteni bárki megteheti. A szerkesztés lehetőségei:

* pull request: minden pull request mergelve lesz a tartalmától függetlenül (legfeljebb a nagyon gázos tartalmakat egy következő commit módosíthatja).
* közvetlen commit: minden bemutatkozás és kötelező kör nélkül lehet kapni közvetlen írás jogot egy issue [kitöltésével](https://github.com/elek/jhacks/issues/new). Pull requestekre válaszlul automatikusan write jog is megy.

A wiki forrás a [github project](https://github.com/elek/jhacks/) master branch-e alatt található, a wiki könyvtár alatti markdown dokumentumokban. A szintaxis megegyezik a Jekyll statikus oldal generátor formátumával (YAML fejléc + markdown szöveg), de az eredeti jekyll site generátor le lett cserélve egy [Java](https://github.com/elek/impremta)-sra. A statikus oldal generálást a [travis-ci](travis-ci.org/elek/jhacks) végzi automatikusan minden commitra.

Lokális repositoryban a ```gradle site``` paranccsal lehet a ```build/_site``` könyvtárba próbából generálni az oldalalkat.

