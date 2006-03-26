---
creationDate        : 2004-09-05 13:55:12 +0200 
author              : admin 
title               : ashkelon 
name                : ashkelon 
layout              : wiki 
path                : ashkelon 
date                : 2006-03-26 01:43:05 +0100 
version             : 1 
creator             : kocka 
---
[http://ashkelon.sourceforge.net/](http://ashkelon.sourceforge.net/)

Az ashkelon egy [javadoc](javadoc.html) eszkoz, ami nem statikus html oldalakat general a forraskodbol, hanem adatbazisba tolti az eredmenyeket.

Elonyei:

*   Projectek kozotti kapcsolatok feloldasa es bongeszhetove tetele
*   Dinamikus bovithetoseg
*   Keresesi lehetosegek (nem am grep meg find meg ilyesmi :) )
*   [maven](maven.html) projectekben az ashkelon descriptor egyszeruen egy "maven ashkelon" paranccsal kigeneralhato

Hibak:

*   Egyszer-ketszer kicsit megzakkantottam, akkor ujra kellett tolteni a contextet :(
*   Cacheli az adatbazis bizonyos elemeit, pl az api-kat nem frissiti minden requesthez, meg idonkent sem, ujra kell startolni a contextet hozza.

Mindenesetre ezek igazan tulelheto hibak, szamomra mar most lenyugdijazta a [javadoc](javadoc.html)-ot. A sajat ashkelon installacionkba szabadidomban toltogetem az forraskodokat, ugyhogy lassankent bovulget. Ha valamit szeretnetek latni benne, akkor irjatok ([kocka](kocka.html) kukac forgeahead pont hu) es ha a license engedi, akkor beteszem.

[http://ashkelon.forgeahead.hu/](http://ashkelon.forgeahead.hu/)
