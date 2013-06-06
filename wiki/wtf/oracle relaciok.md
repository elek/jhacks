---
creationDate        : 2007-11-09 23:20:52 +0100 
author              : kocka 
title               : Mese a gonosz N-N kapcsolatokról 
name                : wtf/oracle relaciok 
layout              : wiki 
path                : wtf/oracle relaciok 
date                : 2007-11-09 23:20:52 +0100 
version             : 1 
creator             : kocka 
---
Ez a mese még az [Oracle](../Oracle.html) 8i korából származik, a régi szép idők ugye :). Egy nagyon nagy terhelésnek kitett alkalmazást fejlesztettünk, amit néhány random helyen izmosan optimalizáltunk, más helyeken (például az architektúra terv) inkáb hanyagoltunk.

Egy ilyen eset volt az, hogy egy komponens programozója bitsorozatban reprezentálta azt hogy egy akármi milyen kategóriákba tartozik, így tényleg villámgyorsan, egy címezéssel, egy shifteléssel és egy XOR művelettel kiderült hogy abba a kategóriába bele tartozik-e. Végülis...

A bug ott tette be a lábát, amikor valaki kitalálta hogy ha már ezt a felhasználó program így reprezentálja, akkor az N-N kapcsolótábla nélkül, az akármi relációban, egy bitstringben tároljuk le. A következő atom hiba azt én követtem el, hogy a specifikációt átvettem és azt mondtam hogy oké, annélkül hogy figyelmesen elolvastam volna. Aztán meg már hiába mérgelődtem, jót röhögek hogy jól megszivattak.
Az oracle-s öregszakival vagy egy hetet izzadtunk a dolgon mire normálisan ment minden lekérdezés és módosítás. Az eredmény: valami félelmetesen lassú lett minden select, új kategória létrehozása horror, amit idáig lehetett indexekkel babrálni, annak itt vége lett és PL/SQL kóddal derült csak ki hogy vajon az akármi passzol-e egy kategóriába.

A dolgot később belátta a management is, és akkor mondták hogy na jó, átírhatjátok, csak akkor már nem akartuk.
