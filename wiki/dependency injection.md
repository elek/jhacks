---
creationDate: 1159477926088 
author: kocka 
contentAuthor: kocka 
title: dependency injection 
contentUpdateDate: 1159477964790 
name: dependency injection 
layout: wiki 
date: 1159477964790 
creator: kocka 
---
A dependency injection az a csodalatos dolog hogy neked nem kell bekodolnod a komponensedbe valami idegolo es kornyezetfuggo modszerrel (pl [JNDI](JNDI.html)) hogy keresse meg a masik komponenseket, hanem maga az [IoC](ioc.html) rendszer beallitja a komponensednek miutan peldanyositotta.

Ket fajtaja ismert:

*   Constructor-based: a konstruktornak passzolunk minden komponens-fuggoseget.
*   Setter based: egyszeru settereket irunk



Mindketto mellett lehet kardozni, de minek. Persze lehet a dolgot keverni, mert pl [spring](spring.html)ben mindkettovel csinalhatod egyszerre :)




