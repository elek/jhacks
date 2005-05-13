---
creationDate        : 2005-05-13 10:57:00 +0200 
author              : kocka 
title               : XQL 
name                : xql 
layout              : wiki 
path                : xql 
date                : 2005-05-13 11:33:05 +0200 
version             : 4 
creator             : kocka 
---
Lekerdezo nyelv [XML](XML.html)-hez, kb mint az [SQL](SQL.html) a relacios adatbazisokhoz (lasd [rdbms](RDBMS.html)). Kapcsolod technologia az [xpath](XPath.html), stb. 

Igazabol elegge korlatolt nyelv, ha az [SQL](SQL.html)lel kell osszehasonlitani, de persze azokban az egszeru esetekben amiket a howto-kba es tutorialokba tesznek meg impresszivnek tunhet. Az avatatlan szem szamara :-D

cikkek:

*   [http://www.ibiblio.org/xql/](http://www.ibiblio.org/xql/)

Lasd meg: [SQL](SQL.html), [XML](XML.html), [XPath](XPath.html), [xindice](xindice.html), [tamino](tamino.html)

# Haxing (Amit [Kocka](kocka.html) gondol errol az egeszrol)

Szoval miert is lenne ez az egesz jo? Tulajdonkeppen nagyon jo arra, hogy hierarchikus adatot ad vissza. Ha elgondolod hogy mekkora lenne:

XML DB (adatbazis layer) -> [XSLT](XSLT.html) transzformaciok pl [cocoon](cocoon.html) (presentation layer) -> browser

Egy lekerdezesbol meg lehetne oldani az egeszet, ha meggondolod nagyon gyors tudna lenni az egesz. Nos erre nem nagyon alkalmas.

Ehhez persze egybol olyan formatumban kellene kerni az XML DBtol, de sajnos vagy nagyon nehez megoldani vagy nem is lehet, igy meg eleg hamar elveszti az ertelmet az egesz :(

Problemak amik az utban allnak (vagy csak en nem ertem oket):

*   Az adatbazisokban vannak adattipusok es operatorok a kulonbozo adatok osszehasonlitasara, de ezt hogy tudom XML-ben hasznalni ahol minden gyakorlatilag string? Pl tegyuk fel amerikai stilusu idiota datumot nyomnak bele az XMl-edbe, es ebbol te meg string osszehasonlitassal se fogod tudni kibogozni hogy melyik volt elobb. pl "event\[@date<'11/11/2005' and @date>'02/02,1998'](Missing.html)", latod hogy nem fog mukodni. Nincs mas, le kell hoznod a teljes tablat, es kliens oldalon vegigvakaraszni, de ezzel agyoncsaptad a teljesitmenyt
*   [SQL](SQL.html)ben joinokkal nagyon egyszeruen tudok riport tablakat generalni. Hogy tudom az XQL lekerdezes adott eredmenyenek adott pontjaira beilleszteni agy masik dokumentum tipus bizonyos elemeit? Mintha nem lehetne.

Szoval a tudomanyom mai allasa szerint igeretes de hasznalhatatlan dolog. Tegyuk hozza hogy a jdk-kba foglalt -es emiatt standard- [XML](XML.html) apik sajnos igazi gagyik.
