---
creationDate        : 2004-12-31 09:50:45 +0100 
author              : kocka 
title               : junit 
name                : junit 
layout              : wiki 
path                : junit 
date                : 2006-06-23 11:35:03 +0200 
version             : 5 
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

A kicsit ujabb es modernebb junit 4 a [java 1.5](java%201.5.html) [annotations](annotations.html) feature-re epit, ezzel kb igy nez ki egy teszt:

```
class TestWhatever { //nem am extends, pojo baszkikaim!!!
    @Test // ez a teszt maga
    public void something() {
    ...
    }
    @Before
    public void elottehivdMarMegLecci() {
    }
}
```

Szoval a jo oreg junit utannaeredt a fiatal tronfosztoknak mint a [testng](testng.html). Ha lassan is. A teljesen uj [pojo](pojo.html) teszteknek szerintem az lesz a vege hogy paran beleirjak a teszteket az objektumokba magaba, tovabblepve pedig majd az eles metodusok teszt metodusokat is fognak hivni. En barmilyen allatsagot el tudok kepzelni :)

Az [IDE](IDE.html)-k altalaban tartalmaznak valamilyen supportot a junit futtatashoz, az [eclipse](Eclipse.html)-ben ez nagyon rulla, a tobbit nem tudom, de itt egy link hozza: [http://www.junit.org/news/ide/index.htm](http://www.junit.org/news/ide/index.htm)

A junit mindenféle portjai:

*   [dbunit](dbunit.html)
*   [httpunit](httpunit.html)
*   satobbiunit

Nekem a kedvencem az amikor egyszerűen csinálsz egy spring context-et és abból szedsz ki bean-eket amiken meghívhatsz a tesztekben metódusokat. Nagyon könnyen ujrafelhasználhatóvá teszi a teszteket.

Cikkek:

*   [Testing Java in an Object-Oriented Way](http://today.java.net/pub/a/today/2006/03/28/testing-java-object-oriented.html) (advanced)

Lasd meg: [XP](XP.html) [test](test.html)
