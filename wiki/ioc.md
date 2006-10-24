---
creationDate        : 2004-08-02 12:24:30 +0200 
author              : kocka 
title               : ioc 
name                : ioc 
layout              : wiki 
path                : ioc 
date                : 2006-10-24 11:49:37 +0200 
version             : 14 
creator             : kocka 
---
__inversion of control__

Az IoC olyan keretrendszert ad a fejlesztett szoftveredhez, ami kezeli komponeneseid fuggosegeit egymason, oszzekapcsolja, konfiguralja esetleg manageli a komponenseket (Lasd meg [COP](COP.html))
Az IoC az amit Martin Fowler atnevezett __Dependency injection__-ra. Mind1, ugy hovja ahogy akarja :)

Alapfilozofia: "Dont call me. I will call you!"

Az [ejb](EJB.html)3 is atvett az IoC tervezesi mintaibol egy keveset.

Altipusok:

*   setter based dependency injection (pl [spring](spring.html))
*   constructor based (pl [picocontainer](picocontainer.html)?)
*   "magad uram ha szolgad nincs" (pl [avalon](avalon.html)) (ezt hivatalosan intrusiv IOC-nek hívják, de ez nagyon csúnya név)


nehany szoftver/framework:

*   [avalon](avalon.html) -> [loom](loom.html)
*   [spring](spring.html)
*   [picocontainer](picocontainer.html)
*   [bigyo](bigyo.html)
*   [OSGi](OSGi.html)
*   a [geronimo](geronimo.html) szerver kernelje ([gbean](Missing.html))

Linkek:

*   [http://today.java.net/pub/a/today/2004/02/10/ioc.html](http://today.java.net/pub/a/today/2004/02/10/ioc.html)
*   [http://www.theserverside.com/articles/article.tss?l=IOCBeginners](http://www.theserverside.com/articles/article.tss?l=IOCBeginners)
*   [http://today.java.net/pub/a/today/2005/07/05/IOCAnnotation.html](http://today.java.net/pub/a/today/2005/07/05/IOCAnnotation.html)


