---
creationDate        : 2004-12-31 09:50:45 +0100 
author              : admin 
title               : junit 
name                : junit 
layout              : wiki 
path                : junit 
date                : 2006-03-26 01:48:18 +0100 
version             : 1 
creator             : kocka 
---
Jeeezusom! Nincs Junit snip!?!?!?!?

[http://junit.org/](http://junit.org/)

Szoval a junit alapveto eszkoz egy onmagara valamit is ado programozo kezeben. Bar eleg egyszerucske. A junit teszteket hajt vegre. Valahogy igy:

```

class TestWhatever extends TestCase {
    //Ez hivodik meg a tesztek elott
    public void setUp() {}
    //Es a tesztek utan
    public void tearDown() {}
    //Es a tesztjeid csupa public es test-tel kezdodo metodusok, pl
    publi void testAkarmi() {
        ...
    }
}

```

Az [IDE](IDE.html)-k altalaban tartalmaznak valamilyen supportot a junit futtatashoz, az [eclipse](Eclipse.html)-ben ez nagyon rulla, a tobbit nem tudom, de itt egy link hozza: [http://www.junit.org/news/ide/index.htm](http://www.junit.org/news/ide/index.htm)

A junit mindenféle portjai:

*   [dbunit](dbunit.html)
*   [httpunit](httpunit.html)
*   satobbiunit

Nekem a kedvencem az amikor egyszerűen csinálsz egy spring context-et és abból szedsz ki bean-eket amiken meghívhatsz a tesztekben metódusokat. Nagyon könnyen ujrafelhasználhatóvá teszi a teszteket.

Lasd meg: [XP](XP.html)
