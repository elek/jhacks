---
creationDate        : 2004-09-05 13:55:12 +0200 
author              : kocka 
title               : ashkelon 
name                : ashkelon 
layout              : wiki 
path                : ashkelon 
date                : 2006-09-08 14:19:23 +0200 
version             : 3 
creator             : kocka 
---
Az ashkelon egy [javadoc](javadoc.html) eszkoz, ami nem statikus html oldalakat general a forraskodbol, hanem adatbazisba tolti az eredmenyeket.

Elonyei:

*   Projectek kozotti kapcsolatok feloldasa es bongeszhetove tetele
*   Dinamikus bovithetoseg
*   Keresesi lehetosegek (nem am grep meg find meg ilyesmi :) )
*   [maven](maven.html) projectekben az ashkelon descriptor egyszeruen egy "maven ashkelon" paranccsal kigeneralhato

Hibak:

*   Egyszer-ketszer kicsit megzakkantottam, akkor ujra kellett tolteni a contextet :(
*   Cacheli az adatbazis bizonyos elemeit, pl az api-kat nem frissiti minden requesthez, meg idonkent sem, ujra kell startolni a contextet hozza.
