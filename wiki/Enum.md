---
creationDate        : 2006-10-15 22:23:36 +0200 
author              : karenin 
title               : Enum 
name                : Enum 
layout              : wiki 
path                : Enum 
date                : 2006-10-15 22:23:52 +0200 
version             : 2 
creator             : karenin 
---
[Java 1.5](java%201.5.html) újítás, típusos felsorolás konstanst lehet vele ízlésesen csinálni.

Definíciója az osztályéhoz hasonló:

```
public enum Evszak {
    TAVASZ, NYAR, OSZ, TEL
}
```

Jó, mert:

*   típusos, azaz lehet Evszak típusú változó, ami csak az adott értékeket veheti fel
*   lehet rá iterátort kapni, és végignézni az értékeit
*   switch-ben használható
*   a háttérben int-ek mennek, ezért gyors
