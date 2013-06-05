---
creationDate: 1167731967062 
author: kocka 
contentAuthor: kocka 
title: WTF/XML reflection 
contentUpdateDate: 1167731967062 
name: WTFXML reflection 
layout: wiki 
date: 1167731967062 
creator: kocka 
---
[Szabadalom](../szabadalom.html)ra erdemes technika, zsenialis nemet-angol-indiai csapattol volt lehetosegem ellesni. :-D

A pattern. Az osztalyod ami egy masik osztaly valamelyik metodusat kell hogy hivja, csinnal egy [XML](../XML.html)-t String-be (kizarolagosan behardcodeolt stringekbol), azt atpasszolja egy utility osztalynak ami az [XML](../XML.html)-t parsolja, ebbol kihalassza azt hogy melyik osztaly, melyik metodusat kell meghivni, sima [reflection](../reflection.html)nel peldanyosit, hiv. az eredmenyt  .toString() metodussal belenyomja egy szinten Stringes [XML](../XML.html)be, es azt visszaadja. Zsenialis reszletekbe is belemenve az exception-okat is nyilvan ugyanigy stringesitve passzolja vissza.

Erdemelne egy [WTF](../WTF.html)-dijjat :)
