---
creationDate        : 2005-01-06 19:22:06 +0100 
author              : kocka 
title               : tablespace 
name                : tablespace 
layout              : wiki 
path                : tablespace 
date                : 2005-01-06 19:22:06 +0100 
version             : 1 
creator             : kocka 
---
Szoval a talbespace egy fizikai helyet jelol, ahova pakolhatod a tablaidat. tipikusan tuning feladat szetpakolgatni oket. A lenyeg az hogy a hozzaferest parhuzmositsd, igy eleg sok idot nyerhetsz.

Szoval altalanossagban, ha jot akarsz:

*   nagy tablak eseten az indexet es a tablat kulon tablespace-be tedd
*   az index tablespace legyen inkabb gyorsabb eszkozon, a tablespace pedig inkab egy biztonsagosabbon
*   join-olas eseten, ha lenyeges a sebesseg, akkor a tablakat kulon eszkozon levo tablespace-be
*   ugyanazon az eszkozon ket kulonbozo tablespace picsafustot nem er, csak cikazik majd koztuk a fej, a pozicionalas meg mindig a leglassabb muvelet lesz.

kb...

Szoval roviden az lenne az idealis, ha minden db objektumodra lenne egy kicsi de gyors vincsid, meg az indexekre is kulon, meghuzva persze tonna memoriaval.<br/>
Na ez az amire nincs penz, nyilvan az optimum az ar/teljesitmeny teren jelentkezik, ezt viszont nehez merni, ugyhogy mondjuk hogy az ugyfel elegedettsegen merjuk az egeszet, azt penzben lehet merni.

Ugyhogy amit fent irtam azt felejtsetek el! :D
