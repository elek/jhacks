---
creationDate        : 2007-09-29 14:17:21 +0200 
author              : renszarv 
title               : GWT 
name                : GWT 
layout              : wiki 
path                : GWT 
date                : 2008-02-23 13:51:17 +0100 
version             : 2 
creator             : karenin 
---
Google Web Toolkit

Rich Client webtool [Google](Google.html) módra. A játék benne, hogy mind a szerver oldali kódot, mind a kliens oldali kódot Java-ban lehet írni. A kliens oldali csomagokat lefordítja egy förtelmesen obfuscált, de működő javascript-re.

Ez a fordítás a szűk keresztmetszet, gyakorlatilag olyasmi élményt nyújt, mint a PDA-kon futó JVM-ekre írni valamit: csak 1.4-et lehet használni, és csak az alap Java API-k vannak meg rajta. Viszont szerver oldalon már bármit használhatunk, amit vidáman lehet kliens oldalról RPC-vel elérni általunk definiált interfészeken keresztül ([doksi](http://code.google.com/webtoolkit/documentation/com.google.gwt.doc.DeveloperGuide.RemoteProcedureCalls.html)) 

A Java-ból fordult komponenseket gyakorlatilag bármilyen HTML-be be lehet szúrni egy egy soros javascript hívás beillesztésével, és onnantól működik a dolog.

Két fajta módban futtatható: Hosted módban nem is fordul le javascript-é, hanem a JVM-en belül indul egy Swinges böngésző, és abban láttjuk az eredményt. Előnye, hogy mivel JVM-en belül vagyunk lehet Debugolni. A Web mode a js-re fordított végleges változatot jelenti.

Az alap telepítésben a hosted mód indításához és a fordításhoz is shell scriptet mellékelnek, ami mind a [maven](maven.html) mind az [ant](ant.html) funok számára ugyanolyan érthetetlen. Azonban lehet Eclipse projektet is generáltatni neki, illetve van hozzá Netbeans plugin (default telepítés Beta repositoryjában).
