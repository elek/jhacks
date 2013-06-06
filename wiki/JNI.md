---
creationDate        : 2004-12-30 10:41:21 +0100 
author              : admin 
title               : JNI 
name                : JNI 
layout              : wiki 
path                : JNI 
date                : 2006-03-26 01:42:43 +0100 
version             : 1 
creator             : kocka 
---
__Java Native Interface__

Egy megoldas arra hogy a java progid tudjon binaris kodot hivni, es forditva. Szoval ha [C](C.html)-s projectedbe akarsz [java](java.html)-t agyazni, vagy forditva, akkor ez neked valo. Viszont altalaban nem egy olyan nagyon jo otlet.

A JNI hivasokon van egy tucat checking overhead, ugyhogy egyaltalan nem biztos hogy megeri [C](C.html)-ben irni a gyakran hivott metodusaidat.

A [java](java.html) [c](C.html)-be agyazasa sem olyan egyszeru dolog mint egy [python](python.html) vagy egyeb nyelv beagyazasa, a [java](java.html) akkor is threadel ha a rajta futo program nem, ez kicsit problemas lehet.
