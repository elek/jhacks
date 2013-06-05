---
creationDate: 1094385312981 
author: kocka 
contentAuthor: kocka 
title: ashkelon 
contentUpdateDate: 1157717963005 
name: ashkelon 
layout: wiki 
date: 1157717963005 
creator: kocka 
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
