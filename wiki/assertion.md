---
creationDate        : 2006-12-06 14:51:56 +0100 
author              : kocka 
title               : assertion 
name                : assertion 
layout              : wiki 
path                : assertion 
date                : 2006-12-06 14:51:56 +0100 
version             : 1 
creator             : kocka 
---
Az assertion a [java 1.4](java%201.4.html) erdekessege volt, az alapgondolat az, hogy ha a VM-et assertion modban futtatod (-ea parameterrel), akkor az assert pontoknal ha a feltetel nem teljesul akkor ott [java.lang.AssertionError](http://docs.oracle.com/javase/7/docs/api/java/lang/AssertionError.html) kepzodik. Ami valoszinuleg kinyirja a [thread](thread.html)edet mert tokre nem illik elkapni.

Kb ennyi a hasznalata:
```
assert 0 < value;
```

Ez nem sok embernek koltozott a szivebe, mert en egyetlen egyszer nem lattam senkit aki hasznalna. Inkab [unit testing](unit%20testing.html). Mindenesetre [test](test.html) futtatashoz erdekes lehetoseg, a semminel meg mindig jobb.


