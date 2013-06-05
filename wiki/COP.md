---
creationDate: 1091002438094 
author: kocka 
contentAuthor: kocka 
title: Component Oriented Programming\\ 
contentUpdateDate: 1122844660250 
name: COP 
layout: wiki 
date: 1122844660250 
creator: kocka 
---
<br/>
Egy nem igazan uj, de meg mindig feljovoben levo programozasi iranyvonal. A lenyege hogy csak komponenseket fejlesztessz, majd ezekbol a komponensekbol allitod ossze a szoftvered. [code reuse](code%20reuse.html)

De hogy kicsit bovebben is legyenek dolgok:<br/>
A dolog valahogy ugy nez ki, hogy te megirod a sajat magad kis vackat, ami egy jol definialt modon erheto el. Ezutan a megfelelo kornyezethez csak azt a kodot kell megirnod, ami az adott kornyezetbol meg tudja hivni az adott komponenst.

A komponens lehet egy osztaly, vagy egy csomag, egy egesz library, vagy egy szoftver, pl egy [rdbms](RDBMS.html) vagy egy [http](HTTP.html) szerver. Szoval komponens az amire azt mondod hogy az az :) Egy komponens altalaban a kovetkezo tulajdonsagokkal rendelkezik:

*   ujrafelhasznalhato tobb alkalmazasban
*   egy meghatarozott feluleten keresztul erheto el, ami elrejti a komponens belso mukodeset
*   es emiatt viszonylag konnyen helyettesitheto mas, ugyanezt a feluletet implementalo komponensekkel. Elmeletileg. Azert ha az [SQL](SQL.html) nyelvre gondolunk mint interface-re [RDBMS](RDBMS.html)ek fele, akkor tudjuk hogy megsem olyan egyszeru a dolog :) (~na jo ez csak elmelet~)



Lasd meg: [RUP](rup.html), [XP](XP.html)
