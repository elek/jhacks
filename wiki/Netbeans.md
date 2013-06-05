---
creationDate: 1091785499619 
author: karenin 
contentAuthor: karenin 
title: Netbeans 
contentUpdateDate: 1180955241965 
name: Netbeans 
layout: wiki 
date: 1180955241965 
creator: kocka 
---
__Netbeans__

http://www.netbeans.org/

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
*   refactoringot nagyon elhanyagolható mértékben támogat. (karenin: Ez az 5-ös szériával nagyon sokat javult, gyakorlatilag minden alap már benne van)
*   nagyon hiányzik belőle az eclipseből jól ismert 3-4 billentyü leütéssel generált setter/getter, az intelligens kód javitó, ami szintén 3-4 billentyü lenyomással beilleszti a ki nem irt cast-okat, és a többi... (karenin: castokat Alt-Enter kiiírja, getter+settert is generál már (sajonos a template-ben nem lehet megadni neki javadocot, de ezt leszámítva korrektül))
*   a UI buildere sajnos egy irányú, tehát nem lehet módositani a kódot tetszés szerint, a netbeans generálja, aztán ha véletlenül mégis belenyúlsz, akkor már ő mossa kezeit. Ez különösen akkor fájó, amikor nem teljesen [triviális](Missing.html) statikus formokat csinál az ember. (karenin: szerintem aki ráérez az ízére, az mindent meg tud benne csinálni, mindenhová be lehet szúrni kódot. Az inkább fájó, hogy nem NetBeans általal generált Swinges formot (amihez nincs .form), csak trükközéssel eszi meg).
*   A Mobility Pack esetén még a kód generáló kiforratlanságával is számolni kell, szeret hibás kódot generálni, módositani csak mértékkel lehet benne, s ami a legfájóbb volt, hogy az esemény kezelő kód beirását egy olyan modális dialogusban kell elvégezni, amiben nincs _semmilyen_ code completion. Most megnézem azt a fejlesztőt, aki mind fejben tartja, hogy éppen a pár tucat változóját, és fieldjét és formját hogyan hivják.



Ami szerintem jó:
*   jó csomagok(pack) vannak, SOA, Mobile, Gui Builder témakörben
*   überkirály, hogy ANT-ra épülnek a projektjei, ezzel olyan dolgokat is meg lehet csinálni egyszerűen, amihez különben plugin kéne (pl. IvY támogatás)
*   Alapból vannak hozzá csomagok(pluginek), amik (szerintem) sokkal jobbak, mint amit innen-onndan Eclipse-hez szerezhetek (pl. appszerver támogatás). Viszont, ha valami nincs benne alapból, ahhoz egyelőre sokkal kevesebb plugint találni. 



Ami gyenge:
*   code convetion támogatása elenyésző
*   Bár sok web/app konténert támogat, ha valamit nem, akkor ahhoz nagyon nehéz összelőcsölni (pl. 5.5-ben Tomcat 6 nem volt)
*   Az Eclipse view rendszere szerintem kicsit okosabb, itt nem lehet megjegyeztetni összerakott ablak állásokat.



</tapasztalatok>



Jelenlegi változat az 5.5/5.5.1 (5.5.1-hez nem adták ki az Enterprise Packet)



Jelenlegi fejlesztési változat: 6.0 újdonságok (várható 2007 őszén)
*   Erősen rágyúrtak az editor képességeire (színesebb, okosabb, ügyesebben találja ki mit akarunk)
*   Schliemann: egy egyszerű(?) szintaxis segítségével könnyel lehet más nyelvekhez editálás (kódszínezés, kódgiegészítés) képességeket passzintani. El is készült egy rakás template.
*   Jackrabbit: újfajta refactor api. Viszonylag egyszerűen lehet majd refactor dolgokat definiálni magunknak (értsd: modul fejlesztés nélkül).
*   Enterprise Pack SOA ([OpenESB](OpenESB.html)) támogatása erősen jó lesz (sok bindinget alapból eszik)
*   Swing Application Framework támogatás
*   JRuby támogatás
