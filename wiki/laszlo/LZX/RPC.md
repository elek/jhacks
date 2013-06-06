---
creationDate        : 2007-06-25 10:59:33 +0200 
author              : kocka 
title               : laszlo/LZX/RPC 
name                : laszlo/LZX/RPC 
layout              : wiki 
path                : laszlo/LZX/RPC 
date                : 2007-09-21 17:44:11 +0200 
version             : 7 
creator             : kocka 
---
A [laszlo/LZX](../../laszlo/LZX.html) nyelv a következő beépített [remote procedure call](../../RPC.html) lehetőségekkel rendelkezik:

*   [soap](../../SOAP.html) / [webservices](../../WebServices.html) ez csak proxizva, azaz a hivás bemegy a prezentációs szerverre és onnan megy ki a tényleges [soap](../../SOAP.html) hivás. Na ezt nem sikerült maradéktalanul működésre bírni.
*   [java](../../java.html) rpc, ezzel meg csak 'public static' dolgokat lehet hívni, ami rettenetesen rossz architektúrát kényszerít ki :(
*   [xml-rpc](../../xml-rpc.html), na ezt is ismerjük, szintén proxizva megy, viszont persze ismertek az xml-rp korlátai
*   [Ajax](../../ajax.html) Legalábbis van XMLHttpRequest objektum, és ezzel lehet ugyanazt csinálni mint javascriptben általában, itt viszont [XML](../../XML.html)-t parsolhatsz mint gép, az azért javascriptben sem csak játék és mese

Igen, kicsit fikagörgetősnek hangzik a fenti, de ezek a tapasztalataim az  [OpenLaszlo](../../Laszlo.html) [RPC](../../RPC.html) lehetőségeivel, és egyébként az egész rendszerük gyenge pontjának tartom.


