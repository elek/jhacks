---
creationDate: 1091022438366 
author: zsoltk 
contentAuthor: zsoltk 
title: millstone 
contentUpdateDate: 1091022485343 
name: millstone 
layout: wiki 
date: 1091022485343 
creator: zsoltk 
---
Egyik kedvencem.

Elerheto a http://www.millstone.org cimen. Erdemes megnezni a Feature Demo nevezetu reszt.

Gondoltma irok rola, de vegulis atemeltem azt (a jol ismert __Copy - Paste__ pattern) amit egy masik wikibe irtam:

Egyszeru library, amivel AWT programozashoz hasonloan lehet HTML alkalmazasokat feljeszteni. Az alapjait egy egyszeru XSLT processzor adja, ami a Java objektumok altal letrehozott XML leirobol csinalja meg a megfelelo HTML oldalt.

A programozasa alapvetoen rendkivul egyszeru. A megfelelo vizualis komponenseket a megfelelo tarolokhoz adogatjuk. Minden tovabbi dolgot az XSLT processzor, ill. a WebAdapterServlet elvegez helyettunk. Nincs szukseg arra, hogy a kulonbozo parametereket nyilvantartsuk, formatumokkal szorakozzunk. Minden adat rendelkezesre all a megfelelo komponensben.

Kulon kiemelendo, hogy minden komponenshez tartoznak kulonbozo esemenyek - a'la .NET - melyeket kezelve adhatunk funkcionalitast a megjeleneshez.

A library felepitese nem tulzottan bonyolult es eleg jol elkulonitett reszekbol all, igy elvileg lehetseges barmilyen konkret megjelenitesi reteg implementalasa. A library 3 fo reszre oszthato:

    * Fuggetlen vizualis kompoenensek
    * Adatkezelo komponensek
    * Konkret megjelenito komponensek

A programozas folyaman nagyreszt a vizualis komponenseket hasznaltam, bar az adatkezelo komponensek is igertesnek tunnek. A konkret megjelenites meg csak HTML outputot tud letrehozni, de ez egyenlore boven elegnek tunik, figyelembe veve, hogy milyen macerat tud okozni egy komolyabb HTML oldal lekezelese.

Fontos megjegyezni, hogy a Xalan es Xerces libek hasznalata erosen ajanlott. A Windows-os J2SE es J2EE tartalmazza a szukseges libeket, de Linux eseten szukseg van a ket fenti lib letoltesere.

Konfiguralasa, debugololasa, deployalasa meglehetosen egyszeru, gyakorlatilag a TXT elolvasasa utan hasznalatba vehetjuk a rendszert.

Elvileg van lehetosegunk arra, hogy a generalt HTML oldal kinezeten valtoztassunk, ne adj isten, teljesen uj layout-ot csinaljunk, de ez azert nem annyira egyszeru. Mindenesetre van ra lehetoseg, de a default megjelenes is meglehetosen jol nez ki.

Egyetlen problemat lattam, ami viszont eleg sulyos. Bar az API rendelkezesre all, a fizetos konyv nelkul eleg sokaig tart, mig az ember kimazsolazza, kiprobalja a rendszer lehetosegeit, beallitasait. Persze ez sem lehetetlen, csak idobe telik.

Osszessegeben szerintem egy nagyon is hasznalhato valami. Intranet jellegu alkalmazasokra mindenfelekeppen. 
