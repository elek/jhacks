---
creationDate        : 2004-12-09 11:31:37 +0100 
author              : kocka 
title               : NPE 
name                : NPE 
layout              : wiki 
path                : NPE 
date                : 2006-12-22 16:36:22 +0100 
version             : 6 
creator             : kanni_baa 
---
núl pojinter ekszepsön

[java.lang.NullPointerException](http://docs.oracle.com/javase/7/docs/api/java/lang/NullPointerException.html)

Le kellett roviditeni mert gyakran fordul elo, es nem kiraj mindig leirni.

Szoval az NPE egy hatalmas feature a java-ban, amikor a hivatkozasod nem mutat semmire, de megis meghivsz rajta egy metodst, akkor nem az egesz alkalmazasod hal meg, legalabbis nem feltetlenul, csak az adott muvelet nem sikerul, es kepzodik egy NPE, amit barhol elkaphatsz. Ha meg nem kapod el akkor kilep az alkalmazasod, vagy terminal a [thread](thread.html)ed, [rollback](Missing.html)el a [tranzakcio](Missing.html)d, ilyesmi...

Amikor meg a suliban halgattam egy tanarom velemenyet a java-rol, akkor megjegyezte hogy annak ellenere hogy javaban nincsenek pointerek, a NPE egy erdekes jelenseg. Talan eleinte NullreferenceExceptionnak kellett volna elnevezni, es akkor ez a felreertes is tiszta lenne. De mi szeretjuk a NPE-t ugy ahogy van.

Erdekessegek:

*   [A 10 year old null pointer bug](http://findbugs.blogspot.com/2006/09/10-year-old-null-pointer-bug.html) ([java 1.6](java%201.6.html) vonatkozasban)


