---
creationDate        : 2005-03-29 09:50:52 +0200 
author              : admin 
title               : PostgreSQL/Features 
name                : PostgreSQL/Features 
layout              : wiki 
path                : PostgreSQL/Features 
date                : 2006-03-26 01:42:51 +0100 
version             : 1 
creator             : kocka 
---
A PostgreSQL sok olyan funkciot nyujt, amit amugy csak a kereskedelmi szerverek nyujtottak: UDF-ek, view-k, triggerek, stb. Mara mar a legtobb onmagara valamit is ado [RDBMS](../RDBMS.html) tudja, ennek ellenere a PostgreSQL ezen felul is kepes valami pluszt nyujtani.<br/>

# Dinamiukus tipusrendszer

A tipus rendszer dinamikus, azaz __CREATE TYPE__ paranccsal sajat tipust hozhatsz letre, amiben sajat formatumoddal tarolhatod az adatokat.<br/>
A PostgreSQL alapbol is tobb hasznos tipust tartalmaz, valamint a kiterjesztesek is adhatnak egyeb szabvanyos adattipusokat, pl [PostGIS](../PostGIS.html).

# Dinamiuks [Postgresql/proceduralis nyelv](../PostgreSQL/proceduralis%20nyelv.html) tamogatas

A tarolt eljaras rendszer is hasonloan __CREATE LANGUAGE__ paranccsal uj [PostgreSQL/proceduralis nyelv](../PostgreSQL/proceduralis%20nyelv.html)et illeszthetsz be.
