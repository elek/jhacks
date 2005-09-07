---
creationDate        : 2004-08-30 15:47:35 +0200 
author              : kocka 
title               : memory leak 
name                : memory leak 
layout              : wiki 
path                : memory leak 
date                : 2005-09-07 16:07:17 +0200 
version             : 5 
creator             : kocka 
---
Olyan memoria terulet, amit a program allokalt, de valamilyen hiba vagy hianyossag miatt akkor sem szabaditja fel es adja vissza a rendszernek, amikor mar nem hasznalja.

A teveszme szerint java-ban nincsenek memory leakek. Valojaban elo lehet allitani, bar nagyon muvi uton. <br/>
Egy gyakori megoldast felvazoltam a [JDBC](JDBC.html) snippen :)<br/>
<br/>
Tipp: ha a [tomcat](tomcat.html)edet N idonkent ujra kell inditanod, akkor memory leakeid vannak az egyik alkalmazasban.

Kulonosen akkor szivas a memory leak, ha (mint altalaban egy [j2ee](j2ee.html) [alkalmazas szerver](Alkalmazas%20Szerver.html)en) tobb alkalmazast futtatsz es az egyik felzabalja a memoriat, igy a tobbi is dobalni fogja az [OOM](OOM.html)eket, igy kicsit nehez kitalalni hogy melyik lehetett a bunos. Erre mellesleg jo lenne valami megoldas, ha az alkalmazasokra kulon be lehetne allitani memoria parametereket.

Lasd: [OOM](OOM.html), [GC](GC.html)


