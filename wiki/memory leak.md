---
creationDate: 1093873655239 
author: kocka 
contentAuthor: kocka 
title: memory leak 
contentUpdateDate: 1126102037508 
name: memory leak 
layout: wiki 
date: 1126102037508 
creator: kocka 
---
Olyan memoria terulet, amit a program allokalt, de valamilyen hiba vagy hianyossag miatt akkor sem szabaditja fel es adja vissza a rendszernek, amikor mar nem hasznalja.

A teveszme szerint java-ban nincsenek memory leakek. Valojaban elo lehet allitani, bar nagyon muvi uton. <br/>
Egy gyakori megoldast felvazoltam a [JDBC](JDBC.html) snippen :)<br/>
<br/>
Tipp: ha a [tomcat](tomcat.html)edet N idonkent ujra kell inditanod, akkor memory leakeid vannak az egyik alkalmazasban.

Kulonosen akkor szivas a memory leak, ha (mint altalaban egy [j2ee](j2ee.html) [alkalmazas szerver](Alkalmazas%20Szerver.html)en) tobb alkalmazast futtatsz es az egyik felzabalja a memoriat, igy a tobbi is dobalni fogja az [OOM](OOM.html)eket, igy kicsit nehez kitalalni hogy melyik lehetett a bunos. Erre mellesleg jo lenne valami megoldas, ha az alkalmazasokra kulon be lehetne allitani memoria parametereket.

Lasd: [OOM](OOM.html), [GC](GC.html)


