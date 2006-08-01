---
creationDate        : 2006-02-08 23:34:14 +0100 
author              : kocka 
title               : maven/maven2 
name                : maven/maven2 
layout              : wiki 
path                : maven/maven2 
date                : 2006-08-01 16:46:55 +0200 
version             : 12 
creator             : kocka 
---
A maven 1 utan egy nagy refactor kovetkezett, nagytakaritas a pom formatumaban valtozasok, ilyesmi.

*   regi maven peldaul egy pluginen keresztul tamogatta a multiprojecteket, ezt a maven 2 alapbol tudja
*   Minden plugin lett, azaz mindener a halozathoz nyul, az alap cucc csak 1 mega, minden mast csak akkor tolt le ha kell.
*   Uj, a regivel termeszetesen inkompatibilis plugin struktura
*   uj repository struktura
*   archetype-ok új projectek villám gyors létrehozására
*   mirrorozhato a repository, nem al meg az elet ha lehal egy szerver: [http://maven.apache.org/guides/mini/guide-mirror-settings.html](http://maven.apache.org/guides/mini/guide-mirror-settings.html)
*   van hozza proxy szoftver is [http://maven-proxy.codehaus.org/](http://maven-proxy.codehaus.org/)

[Test](../test.html) frameworkbol tamogatja a [junit](../junit.html) 3.8-at es a [testNG](../testng.html)-t, [junit](../junit.html) 4-el is meg lehet hajtani eppen, ha pont ugyanugy nevezed az metodusokat ahogy 3.8 alatt. [Test/Categorization](../Test/Categorization.html) nincsen sajnos, pedig de jo is lenne :)

Cikkek:

*   [Get the most out of Maven 2 site generation](http://www.javaworld.com/javaworld/jw-02-2006/jw-0227-maven_p.html)
*   [Maven 2.0: Compile, Test, Run, Deploy, and More](http://www.onjava.com/lpt/a/6528)
*   [The Maven 2 POM demystified](http://www.javaworld.com/javaworld/jw-05-2006/jw-0529-maven.html)

linkek:

*   [http://mvnrepository.com/](http://mvnrepository.com/) (ha valamilyen artifactot keresel, hasznos)

__konyv__:

*   Egy regisztracio utan [letoltheto konyv](http://www.mergere.com/m2book_download.jsp). Beleolvasva: nem rossz.

Egy egesz jol fejlodo [eclipse](../Eclipse.html) [eclipse/plug-in](../Eclipse/Plug-in.html) hozza: [http://m2eclipse.codehaus.org/](http://m2eclipse.codehaus.org/)

Lasd: [maven](../maven.html), [maven/maven1](../maven/maven1.html), [build](../build.html)
