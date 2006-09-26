---
creationDate        : 2004-08-06 11:44:59 +0200 
author              : karenin 
title               : Netbeans 
name                : Netbeans 
layout              : wiki 
path                : Netbeans 
date                : 2006-09-26 16:23:59 +0200 
version             : 7 
creator             : kocka 
---
__Netbeans__

[http://www.netbeans.org/](http://www.netbeans.org/)

Egy free [IDE](IDE.html) a [sun](Sun.html) kornyekerol. A NetBeans rengeteg alap pluginnal jon, ami miatt nagyon gyorsan bele lehet tanulni a hasznalataba:

*   Web projectek tamogatasa (pl [jsp](JSP.html) editor)
*   [J2ME](j2me.html) projectek

Ha nincs savszelesseged, akkor [ingyen kerhetsz](http://www.netbeans.org/about/cd-form.html) egy netbeans cd-t. Igaz ami CD-n van az mindig elavult, de azert rendes toluk :)

Mivel a felulete swinges, meglevo alkalmazasokat is konnyen lehet integralni bele. A Plugin felulete viszont allitolag egyszerubb mint az [Eclipse](Eclipse.html)-e.

A netbeans 4.s-es szeriatol a leglenyegesebb ujitas volt benne az [ant](ant.html) hasznalata a projectmanagementre, igy a kodod [ide](IDE.html)-tol fuggetlenul barhol [build](build.html)elheto annelkul hogy a fejlesztoknek foglalkoznia kellene vele.

A netbeans mogott a [SUN](Sun.html) all, ugyanugy mint az [eclipse](Eclipse.html)+[IBM](IBM.html) paros eseteben fizetos szoftvereket fejlesztenek a free alapra.<br/> A "netbeans vs [eclipse](Eclipse.html)" flamewar kb olyan magassagokba csap mint a "[linux](Linux.html) vs [windows](Windows.html)" es a "vim vs joe". (lasd: [haboru](haboru.html))

<flame> [renszarv](renszarv.html): viszont itt egyértelmü, hogy kinek van igaza :D</flame>

<tapasztalatok>
 Viccet félretéve, a netbeans előnyére lehet mondani, hogy jó pár ügyes wizardal, templatetel rendelkezik, s ha a drag & drop éppen müködik, akkor gyorsan lehet benne haladni, viszont... S itt sajnos egy legalább olyan hosszú lista következik: 

*   refactoringot nagyon elhanyagolható mértékben támogat.
*   nagyon hiányzik belőle az eclipseből jól ismert 3-4 billentyü leütéssel generált setter/getter, az intelligens kód javitó, ami szintén 3-4 billentyü lenyomással beilleszti a ki nem irt cast-okat, és a többi...
*   a UI buildere sajnos egy irányú, tehát nem lehet módositani a kódot tetszés szerint, a netbeans generálja, aztán ha véletlenül mégis belenyúlsz, akkor már ő mossa kezeit. Ez különösen akkor fájó, amikor nem teljesen [triviális](Missing.html) statikus formokat csinál az ember.
*   A Mobility Pack esetén még a kód generáló kiforratlanságával is számolni kell, szeret hibás kódot generálni, módositani csak mértékkel lehet benne, s ami a legfájóbb volt, hogy az esemény kezelő kód beirását egy olyan modális dialogusban kell elvégezni, amiben nincs _semmilyen_ code completion. Most megnézem azt a fejlesztőt, aki mind fejben tartja, hogy éppen a pár tucat változóját, és fieldjét és formját hogyan hivják.

</tapasztalatok>

 
