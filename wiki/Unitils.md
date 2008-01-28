---
creationDate        : 2007-12-20 19:28:04 +0100 
author              : kocka 
title               : Unitils 
name                : Unitils 
layout              : wiki 
path                : Unitils 
date                : 2008-01-28 17:15:18 +0100 
version             : 4 
creator             : zmb 
---
Roviden: mindenfele hasznos kiegeszites [junithoz](junit.html) es [testnghez](testng.html). [DBUnit](dbunit.html), [EasyMock](Missing.html), [Spring](spring.html), [Hibernate](Hibernate.html) tamogatas is van benne.

Ficsorok:

*   [Reflection](reflection.html) API segitsegevel objektumok osszehasonlitasa.
*   Collection objektumok osszehasonlitasa, sorrendtol fuggetlenul
*   Annotacioval lehet jelezni, hogy egy test case-hez, vagy egy teszthez tartozik valami dataset.
*   Ugyancsak annotacioval megadhato egy dataset, amit osszevet az adatazissal. Marha kenyelmes, ha valami adatbzis modositast akarsz tesztelni
*   Megadhato neki kulso sql file, amit berant a teszt elott (igy up to date tarthato a dev adatbazis)
*   Annotacioval beinjektalhato [spring](spring.html) AppContext, es bean
*   Megintcsak annotacioval jelezheto, h az ojektum egy mock, raadasul a teszt vegen hivja magatol a verify-t, igy azzal se nem kell torodni.
*   [Hibernate](Hibernate.html) mappinget is tud csekkolni, de aztat nem probaltam meg

[TODO](TODO.html): valami osszefuggobb leirast csiholni ebbol az egeszbol
