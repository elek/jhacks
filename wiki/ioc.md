---
creationDate        : 2004-08-02 12:24:30 +0200 
author              : tvik 
title               : Inversion of Control 
name                : ioc 
layout              : wiki 
path                : ioc 
date                : 2008-02-05 13:15:34 +0100 
version             : 17 
creator             : kocka 
---
Az IoC olyan keretrendszert ad a fejlesztett szoftveredhez, ami kezeli komponeneseid fuggosegeit egymason, oszzekapcsolja, konfiguralja esetleg manageli a komponenseket (Lasd meg [COP](COP.html)).
Ugy 4-5 evvel ezelott par ember agymenese volt, utanna ugy 1-2 evvel ezelottig hype lett, es azota szerintem mainstream technologia, szoval aki kicsit is ad magara az ismeri.
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
*   [hivemind](hivemind.html) ([tapestry](tapestry.html))
*   a [geronimo](geronimo.html) szerver kernelje ([gbean](Missing.html))
*   [guice](guice.html) a Google-től.

Linkek:

*   [http://today.java.net/pub/a/today/2004/02/10/ioc.html](http://today.java.net/pub/a/today/2004/02/10/ioc.html)
*   [http://www.theserverside.com/articles/article.tss?l=IOCBeginners](http://www.theserverside.com/articles/article.tss?l=IOCBeginners)
*   [http://today.java.net/pub/a/today/2005/07/05/IOCAnnotation.html](http://today.java.net/pub/a/today/2005/07/05/IOCAnnotation.html)


