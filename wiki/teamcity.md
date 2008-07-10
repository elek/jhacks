---
creationDate        : 2008-03-05 10:33:58 +0100 
author              : kocka 
title               : teamcity 
name                : teamcity 
layout              : wiki 
path                : teamcity 
date                : 2008-07-10 15:17:56 +0200 
version             : 5 
creator             : kocka 
---
[http://www.jetbrains.com/teamcity/](http://www.jetbrains.com/teamcity/)

Egy sajnos nem free (és igen drága) [continuous integration](Continuous%20Integration.html) szerver. Elosztottan működik, build agentek tudnak a központi szerverrel kommunikálni, ezek a build agentek rendelkezhetnek például különböző attribútumokkal - mint [operációs rendszer](Operacios%20rendszer.html) - ami alapján beállíthtod hogy a projected milyen build agenten szeretne buildelődni.
Néhány cukor:

*   [IDE](IDE.html): [eclipse](Eclipse.html) és [idea](IDEA.html) integráció
*   [version control](version%20control.html): a mainstream cuccokon kívül támogatja a perverz marhaságokat is ([perforce](perforce.html), [vss](sourcesafe.html) például ez ut=bbi nekem nem működött jól)
*   Nem csak azt követi, hogy sikeres volt-e a build, hanem statisztikákat is vezet arról hogy a tesztek milyen arányban mentek át
*   Csapatmunka támogatás - vállalhatod például a felelősséget egy build hibájáért
*   Belül [spring](spring.html)ből van :)
*   Ha a teszt elfailel, automatikusan újrapróbálhatja X idővel később. Például integrációs teszteknél nagyon hasznos, amikor külső szolgáltatásokat hívogatunk, és ezek a külső szolgáltatások persze néha lerohadnak.


