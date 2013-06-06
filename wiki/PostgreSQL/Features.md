---
creationDate        : 2005-03-29 09:50:52 +0200 
author              : kocka 
title               : PostgreSQL/Features 
name                : PostgreSQL/Features 
layout              : wiki 
path                : PostgreSQL/Features 
date                : 2007-11-01 10:41:00 +0100 
version             : 3 
creator             : kocka 
---
A PostgreSQL sok olyan funkciot nyujt, amit amugy csak a kereskedelmi szerverek nyujtottak: UDF-ek, view-k, triggerek, stb. Mara mar a legtobb onmagara valamit is ado [RDBMS](../RDBMS.html) tudja, ennek ellenere a PostgreSQL ezen felul is kepes valami pluszt nyujtani.<br/>

# Dinamiukus tipusrendszer

A tipus rendszer dinamikus, azaz __CREATE TYPE__ paranccsal sajat tipust hozhatsz letre, amiben sajat formatumoddal tarolhatod az adatokat.<br/>
A PostgreSQL alapbol is tobb hasznos tipust tartalmaz, valamint a kiterjesztesek is adhatnak egyeb szabvanyos adattipusokat, pl [PostGIS](../PostGIS.html).

# Dinamiuks [Postgresql/proceduralis nyelv](../PostgreSQL/proceduralis%20nyelv.html) tamogatas

A tarolt eljaras rendszer is hasonloan __CREATE LANGUAGE__ paranccsal uj [PostgreSQL/proceduralis nyelv](../PostgreSQL/proceduralis%20nyelv.html)et illeszthetsz be.

# Inheritance

Ez szerintem egy igazán figyelemre méltó dolog volt a postgresql 7.x szériában, és persze a 8.x is tarjta vele a kompatibilitást, de nem igazán fejlesztenek rá semmit se már (tudtommal). A relációk közt, ugynúgy mint például az [OR Mappinggal](../OR%20Mapping.html) rájuk mappelt osztályok közt öröklődést lehetett megvalósítani. Az azt jelenti hogy ha B reláció A reláció leszármazottja, akkor ha B-be beteszel egy rekordot, akkor annak a (projekciója, nyilván) látszani fog A relációban is.

Ez egy érdekes dolog lett volna, [RDBMS](../RDBMS.html) szintre letolni a öröklődések megoldását, ehelyett az terjedt el, hogy az [OR Mapping](../OR%20Mapping.html) komponensek a két ismert alkalmazásszintű módszerrel dolgoznak.

# [XML](../XML.html)

A 8.3-as verzió érkezik beépített XML típus támogatással. Meglátjuk konkrétan mit tud...
