---
creationDate: 1105609202473 
author: kocka 
contentAuthor: kocka 
title: Laszlo 
contentUpdateDate: 1213084857068 
name: Laszlo 
layout: wiki 
date: 1213084857068 
creator: zsoltk 
---
Rich Internet Application development framework.



Egy [flash](flash.html) oldalakat generalo cucc (persze hivatalosan [dhtml](Missing.html) rintime is van, es stabil is), sajat xml nyelvvel [laszlo/lzx](laszlo/LZX.html), [OOP](oop.html) design, satobbi. Ja es [XML](XML.html)alapu, nem ar ismerni nemi [XPath](XPath.html)t se hozza. Az eredmeny nagyon designos flash, mindenhol animalt, a juzerek kotelesek imadni, foleg ha meg valami funkcionalitas is akad mogotte.

[laszlo/LZX](laszlo/LZX.html) cuccokat a laszlo compilerrel atfordithatod [bytecode](bytecode.html)ba, vagy futtathatod siman a prezentacios szerveren ami szukseg szerint fogja forditani neked. Nehany hatarozottan pozitiv [rpc](RPC.html) feature-t meg kielemnek: [java](java.html) hivasok, persze remote, [xml-rpc](xml-rpc.html), [soap](SOAP.html). Ezzel azert vannak szivasok helyenkent, a [soap](SOAP.html) api kicsit nehezen hasznalhato, a [java](java.html) [rpc](RPC.html) session-onkent egy objektumot csinal. (valahogy jobb otletnek tartanam az [ioc](ioc.html)-s service objektumok hasznalatat, de megoldhato, csak nagyon harcos :) )



Sajat [test](test.html) rendszere is van lzunit neven.

# [IDE](IDE.html) support

*   [alfás eclipse plugin](http://www.syte.ch/en/laszlo.xml)
*   [pénzéhes eclipse plugin](http://www.spket.com/laszlo.html)

# Linkek

*   http://www.openlaszlo.org/
*   http://www.laszlosystems.com/lps/laszlo-in-ten-minutes/ (nagyon impressziv demok)
*   [Gliffy, egy izmosabb demo arrol hogy miket lehet belole kihozni](http://www.gliffy.com/gliffy/)

# [Maven](maven.html)



Nem volt teljesen evidens hogy hogyan lehet bele fejleszteni [maven](maven.html) alatt, de kikiserleteztem es irtam hozza egy archetype-ot is. Szoval egyszeruen maven-war-plugin hasznalataval, csak oda kell figyelni hogy a 2.0 verzio meg legyen belole mert a regebbiek nem eleg jok hozza. A maven fuggosegek koze tegyel be egyszeruen egy fuggoseget az openlaszlo war file-nak, ezt a war plugin ki fogja csomagolni neked, a sajat web.xml-ed pedig felulvaghatja az openlaszlo cuccot, az lzx filejaidat pedig egyszeruen benyomhatod a src/main/webapp ala. egy egyszeru jetty6:run azonnal uzemelo openlaszlo szervert hoz neked letre. Szoval bevetheto, csak kiserletezni kellett sokat, mert ez sehol nincs leirva.








