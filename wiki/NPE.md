---
creationDate        : 2004-12-09 11:31:37 +0100 
author              : admin 
title               : NPE 
name                : NPE 
layout              : wiki 
path                : NPE 
date                : 2006-03-26 01:42:47 +0100 
version             : 1 
creator             : kanni_baa 
---
núl pojinter ekszepsön

[java.lang.NullPointerException](http://docs.oracle.com/javase/7/docs/api/java/lang/NullPointerException.html)

Le kellett roviditeni mert gyakran fordul elo, es nem kiraj mindig leirni.

Szoval az NPE egy hatalmas feature a java-ban, amikor a hivatkozasod nem mutat semmire, de megis meghivsz rajta egy metodst, akkor nem az egesz alkalmazasod hal meg, legalabbis nem feltetlenul, csak az adott muvelet nem sikerul, es kepzodik egy NPE, amit barhol elkaphatsz. Ha meg nem kapod el akkor kilep az alkalmazasod, vagy terminal a [thread](thread.html)ed, [rollback](Missing.html)el a [tranzakcio](Missing.html)d, ilyesmi...

Amikor meg a suliban halgattam egy tanarom velemenyet a java-rol, akkor megjegyezte hogy annak ellenere hogy javaban nincsenek pointerek, a NPE egy erdekes jelenseg. Talan eleinte NullreferenceExceptionnak kellett volna elnevezni, es akkor ez a felreertes is tiszta lenne. De mi szeretjuk a NPE-t ugy ahogy van.
