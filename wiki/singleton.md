---
creationDate        : 2006-11-16 11:33:34 +0100 
author              : kocka 
title               : singleton 
name                : singleton 
layout              : wiki 
path                : singleton 
date                : 2006-11-16 11:33:34 +0100 
version             : 1 
creator             : kocka 
---
A Singleton [Design Pattern](Missing.html)

Lenyege: az alkalmazasban csak egyetlen egy peldanya lehessen az adott objektumnak:

Megvalositas:
Tobbnyire ugy tortenik hogy a konstruktort privatta teszed, aztan csinalsz egy metodust amin keresztul vagy letrehozod az objektumot vagy visszaadod az egyetlen, mar letrehozott cuccot. Kb igy:

```
class MySingleton {
private MySingleton() {}

MySingleton instance;

public static synchronized MySingleton getInstance() {
 if(instance == null){
  instance = new MySingleton()
 }
 return instance;
}

```

Hat ennyi. Valojaban persze csak az adott [classloader](classloader.html)en belul lesz singleton, de ez tobbnyire eleg.

Mivel kicsit nehezen kezelheto eset, furi refaktoralni is, ezert [antipattern](antipattern.html) dijra lett eloterjesztve tobb esetben is.
