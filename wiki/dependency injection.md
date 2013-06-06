---
creationDate        : 2006-09-28 23:12:06 +0200 
author              : kocka 
title               : dependency injection 
name                : dependency injection 
layout              : wiki 
path                : dependency injection 
date                : 2006-09-28 23:12:44 +0200 
version             : 2 
creator             : kocka 
---
A dependency injection az a csodalatos dolog hogy neked nem kell bekodolnod a komponensedbe valami idegolo es kornyezetfuggo modszerrel (pl [JNDI](JNDI.html)) hogy keresse meg a masik komponenseket, hanem maga az [IoC](ioc.html) rendszer beallitja a komponensednek miutan peldanyositotta.

Ket fajtaja ismert:

*   Constructor-based: a konstruktornak passzolunk minden komponens-fuggoseget.
*   Setter based: egyszeru settereket irunk

Mindketto mellett lehet kardozni, de minek. Persze lehet a dolgot keverni, mert pl [spring](spring.html)ben mindkettovel csinalhatod egyszerre :)


