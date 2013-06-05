---
creationDate: 1091783189394 
author: kocka 
contentAuthor: kocka 
title: loom 
contentUpdateDate: 1110185867344 
name: loom 
layout: wiki 
date: 1110185867344 
creator: kocka 
---
![image](http://loom.codehaus.org/images/loom-logo.png)

__Loom__

http://loom.codehaus.org/

# Roviden

Valoszinuleg a legtobb szerver oldali funkcionalitast nyujto [avalon](avalon.html) container. Van benne [JMX](JMX.html), hot deploy, meg minden mi szem szajnak ingere.
[codehaus](codehaus.html) project, a [phoenix](phoenix.html) forkja es utodprojectje. Futtat [avalon](avalon.html) es [dna](DNA.html) es [picocontainer](picocontainer.html) komponenseket is.

# Tortenelem

Az [Avalon](avalon.html) es a [Phoenix](phoenix.html) akkor kezdodott, amikor meg teljesen gyerekcipoben jart az egesz [IoC](ioc.html) es [COP](COP.html) tema, valahogy a 90es evek kozepen. Azok akik mar akkor belatak a szuksegesseget, azok hamar raaltak, es igy sok nagy es kicsi felhasznalot orokolt meg a [Phoenix](phoenix.html) projecttol a loom is. Az avalon viszont egy nem igazan kedvelt API lett, reszben a "intrusive" [IoC](ioc.html) nepszerutlenedese, reszben pedig az [avalon](avalon.html) projecten belul lezajlott belhaboruk miatt, igy a loomnak most kemenyen kell majd hajtania hogy ujra mainstream rendszer lehessen.

# Reszletek

A [metaclass](MetaClass.html) library-t hasznalja a komponens metainformaciok tarolasara, bar erti a regi .xinfo-s felallast is, igy a phoenix alkalmazasok futtathatoak rajta. Persze itt meg kell jegyezni hogy a loom kidobta a phoenix legtobb dependency-jet, igy valoszinu hogy bele kell pakolni a csomagba azokat is. Egy mc-el pillanatok alatt :)

Elinditottak egy loom applications repository-t is, ahova kerni lehet linkek felvetelet, esetleg ha jo fiu vagy es erdekes a cucc amit irni akarsz, kapsz egy [CVS](CVS.html) hozzaferest is egy repository aghoz.<br/>

*   http://loom.codehaus.org/loom+applications (ezt olvasd el)
*   irc://irc.codehaus.org/#jcontainer (itt vannak az arcok akikkel beszelni kell)

Jelenleg meg kicsit ures, de lesz ez meg maskent, nekem is van 3 loom alapu fejlesztesem.
