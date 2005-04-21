---
creationDate        : 2005-04-21 14:19:48 +0200 
author              : kocka 
title               : j4sql/Annotations vs javadocs 
name                : j4sql/Annotations vs javadocs 
layout              : wiki 
path                : j4sql/Annotations vs javadocs 
date                : 2005-04-21 14:20:34 +0200 
version             : 3 
creator             : kocka 
---
Mindket megoldasnak megvan a maga elonye es hatranya:

[annotations](../annotations.html):

*   (+) a binarisbol is olvashato a metainformacio
*   (-) viszont fuggoseg alakult ki a [j4sql](../j4sql.html) annotaciok es az alkalmazas kozott
*   (-) [java 1.5](../java%201.5.html) fuggoseg, nem sokan hajtanak meg ilyet, adatbazisban meg meg kevesebben

[javadoc](../javadoc.html) tagek:

*   (-) a deployment adat csak forrasbol szedheto ki, vagy egy olyan library-vel is  bepakolhato a classfileokba mint a [metaclass](../MetaClass.html), csak akkor vegkep eltavolodtunk a standardtol
*   (+) nincs fuggoseg, siman hasznalhato ms megoldasokkal egyut.

Ugyhogy a megoldas: decoupling :) nyilvan. Mind a ketto lehetseges lesz, igy kicsit bolonyultabb, de abszolult rugalmas lesz.

lasd meg: [qdox](../QDox.html)
