---
creationDate        : 2007-12-20 19:28:04 +0100 
author              : zmb 
title               : Unitils 
name                : Unitils 
layout              : wiki 
path                : Unitils 
date                : 2007-12-20 19:28:04 +0100 
version             : 1 
creator             : zmb 
---
Roviden: mindenfele hasznos kiegeszites junithoz es testnghez. DBUnit, EasyMock, Spring, Hibernate tamogatas is van benne.

Ficsorok:

*   Reflection API segitsegevel objektumok osszehasonlitasa.
*   Collection objektumok osszehasonlitasa, sorrendtol fuggetlenul
*   Annotacioval lehet jelezni, hogy egy test case-hez, vagy egy teszthez tartozik valami dataset.
*   Ugyancsak annotacioval megadhato egy dataset, amit osszevet az adatazissal. Marha kenyelmes, ha valami adatbzis modositast akarsz tesztelni
*   Megadhato neki kulso sql file, amit berant a teszt elott (igy up to date tarthato a dev adatbazis)
*   Annotacioval beinjektalhato spring AppContext, es bean
*   Megintcsak annotacioval jelezheto, h az ojektum egy mock, raadasul a teszt vegen hivja magatol a verify-t, igy azzal se nem kell torodni.
*   Hibernate mappinget is tud csekkolni, de aztat nem probaltam meg

TODO: valami osszefuggobb leirast csiholni ebbol az egeszbol