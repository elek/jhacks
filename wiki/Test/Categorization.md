---
creationDate        : 2006-08-01 17:03:03 +0200 
author              : kocka 
title               : Test/Categorization 
name                : Test/Categorization 
layout              : wiki 
path                : Test/Categorization 
date                : 2006-12-06 15:12:34 +0100 
version             : 7 
creator             : kocka 
---
A tortenet kicsit kavar, mert aki csak [pojo](../pojo.html)kat kodol, az neha meg van gyozodve rola hogy a tesztek cefet gyorsan lefutnak, minden platformon, ugyhogy kar is kategorizalni egy project tesztjeit, le lehet barmelyik buildben futtatni siman.

Hat a vilag sajnos nem ennyire idealis, pedig de szep is lenne.

Vannak ugyanis kulonbozo [platform](../Missing.html)fuggo szolgaltatasok amikre egy alkalmazas epul, peldaul [rdbms](../RDBMS.html) platform meg [alkalmazas szerver](../Alkalmazas%20Szerver.html) platform, amiket szinten tesztelni kell de nem lehet minden kornyezetben vegrehajtani a tesztet (pl ha nincs orakulum installalva), meg a tesztek is tobbfelek, szoval ha mas mod nincs ra, akkor kategorizacioval elvalaszthato hogy mikor melyik tesztnek kell lefutnia.

Ez egy viszonylag uj koncepcio, peldaul a [junit](../junit.html)ban is csak a 4.1-tol van kategorizacio, [IDE](../IDE.html) support ilyesmihez meg egyaltalan nincs. A [TestNG](../testng.html) tamogatja, sajnos a [testng](../testng.html)t viszont masok nem annyira mint a [junit](../junit.html)ot.

Linkek:

*   [Implementing Test Categorization](http://thediscoblog.com/?p=19) ([ant](../ant.html)tal)
*   [Introduction to build profiles](http://maven.apache.org/guides/introduction/introduction-to-profiles.html) ([maven/maven2](../maven/maven2.html)) egy elegans mod a test categorization kivitelezesere [surefire pluginnal](http://maven.apache.org/plugins/maven-surefire-plugin/examples/testng.html) (persze csak [testng](../testng.html) eseteben :( )
*   [Use test categorization for agile builds](http://www.ibm.com/developerworks/java/library/j-cq10316/index.html?ca=drs-)
*   [Test Categorization Techniques with TestNG](http://dev2dev.bea.com/pub/a/2006/09/testng-categorization.html)


