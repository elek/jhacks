---
creationDate        : 2005-05-03 10:03:43 +0200 
author              : kocka 
title               : Vector 
name                : Vector 
layout              : wiki 
path                : Vector 
date                : 2005-05-03 10:03:43 +0200 
version             : 1 
creator             : kocka 
---
[java.util.Vector](http://docs.oracle.com/javase/7/docs/api/java/util/Vector.html)

Egyfajta collection, a kezdok szivesen hasznaljak valtozo meretu tombnek, __DE EZ TOBBNYIRE HELYTELEN, A KEZUKRE KELLENE CSAPNI EGY HUSZ KILOS KALAPACCSAL__, mert a Vector szinkronizalt, emiatt lassu es csak akkor kellene hasznalni ha tobb thread ferhet hozza, ha csak egy thread latja, akkor jobb az pl [java.util.ArrayList](http://docs.oracle.com/javase/7/docs/api/java/util/ArrayList.html)et hasznalni.
