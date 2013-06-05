---
creationDate: 1198175284633 
author: kocka 
contentAuthor: kocka 
title: Unitils 
contentUpdateDate: 1201536918959 
name: Unitils 
layout: wiki 
date: 1201536918959 
creator: zmb 
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
