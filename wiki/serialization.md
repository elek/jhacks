---
creationDate        : 2005-01-17 10:57:06 +0100 
author              : kocka 
title               : serialization 
name                : serialization 
layout              : wiki 
path                : serialization 
date                : 2006-09-28 22:57:25 +0200 
version             : 5 
creator             : kocka 
---
Objektumok kiirasa stream-be, illetve objektumok letrehozasa stream-bol. Itt kell megemliteni a meltan ritkan hasznalt _transient_ kulcsszot a [java](java.html)ban, amit ha rahuzol egy field-re, akkor az nem fog reszt venni a serializacioban. Nem kap erteket, nem megy ki a file-ba. Mellesleg ez az egesz egyebkent [reflection](reflection.html)nal mukodik.

Amit erdemes ismerni vele kapcsolatban az ugyebar a [java.io.ObjectInputStream](http://docs.oracle.com/javase/7/docs/api/java/io/ObjectInputStream.html) es [java.io.ObjectOutputStream](http://docs.oracle.com/javase/7/docs/api/java/io/ObjectOutputStream.html), valamint vannak alternativak a peldaul a kivallo [xstream](xstream.html), vagy hasznalhatsz mas [XML object mapping](XML%20object%20mapping.html)et, amik ugyan sajat apit kovetnek, de a binaris stream helyett [XML](XML.html)t hasznalnak, ami emberileg is editalhato, ha ugy adodik.

Utalom amikor behardcodeoljak a serialization-t [persistence](persistence.html) helyett. ([Kocka](kocka.html))


