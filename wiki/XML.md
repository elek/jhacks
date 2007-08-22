---
creationDate        : 2004-11-17 22:36:54 +0100 
author              : kocka 
title               : eXtended Markup Language 
name                : XML 
layout              : wiki 
path                : XML 
date                : 2007-08-22 17:56:34 +0200 
version             : 10 
creator             : boci 
---
A [Word Wide Web Consurtium](http://www.w3.org) altal kiadott adatdefinicios szabvany. Egyszeru szabalyainak kosoznhetoen igen gyorsan elterjedt lett. [XSLT](XSLT.html) segitsegevel az adatstruktura konnyen megjelenitheto.

Az XML egy idoben sajnos overhype-olt technologia volt, sokan feledketzek meg a korlatairol, es tettek olyan helyekre ahova nem valo. (Es mindezt teszik maig is joparan)<br/>
Mindig tartsd szemelott hogy az XML egy portolhato adatformatum, de a parsolasa lassu. A rendszer hatarain atlepni vele konnyu es jo, a rendszeren belul nehez es rettenetes.

Szivasok az XML-ben: 

*   amikor peldaul a parsered mindenkeppen validalni akarja a [dtd](DTD.html)vel, de vagy offline vagy vagy a szerver eppen pihen. Ilyenkor kicsit pocsolhetsz rajta hogy vajon mi is romolhatott el... 
*   A [java](java.html) default xml apik olyan mint egy horrorfilmsorozat.

Parsolók:

*   [DOM](dom.html) szabványos dom fát épít
*   [SAX](sax.html) push parser, hatékonyabb, de kényelmetlenebb
*   [StAX](StAX.html) pull parser leghatékonyabb, és azért a SAX-nál kicsit kényelmesebb

Egyéb apik:

*   [JAXB](jaxb.html) xml és objektum hierarchia közötti meppelést csinál
*   [JAXP](Missing.html) az alap parzoló api
*   [JAXR](JAXR.html) registryket (pl. [UDDI](UDDI.html)) elérő api
*   [JAXM](Missing.html) ezt még sose használtam, de ha vizsgán kérdezik, hogy mi ez, és benne van a message-ing szó, akkor ezt kell kiválasztani :)
*   [xpp3](Missing.html) nem callbackol, nem épít felhőkarcolókat, szedd ki magad és csinálj vele amit akarsz. Imádnivalóan gyors, csak azért persze kicsit fáj a kódot összevacakolni hozzá, kicsit procedurális lesz

[webservices](WebServices.html) szagú XML közeli API-k

*   [JAX-RPC](JAX-RPC.html) Web Services kliens/server API. Deprecated
*   [JAX-WS](JAX-WS.html) A JAX-RPC utódja. Annotációkkal web servicek. Szabványos lett, amit az [XFire](xfire.html) már régen tudott.
*   [SAAJ](SAAJ.html) SOAP-os attachmenteket kezel.  

Linkek:

*   [http://www.w3.org/XML/](http://www.w3.org/XML/)
*   alternativ DOM implementaciok: [jdom](jdom.html), [dom4j](dom4j.html)

Lasd: [w3c](w3c.html), [xslt](XSLT.html)

# XML DB

Az XML egy ideje bevete magat az adatbazis technologiak koze is, aminek itathatatlanul van nagyon sok elonye, de mivel meg mindig eleg uj dolognak minosul, igazabol a hatranyai gyakran jelentosebbek.

A rabbi is altalaban azt mondja ezekről, hogy nagyon frankók, csak sajnos a relációs adatbázis kezelő gyártóknak már sokkal nagyon tapasztalataik vannak, úgy hogy általában a megbízhatóság kedvéért inkább parzolunk és meppelünk.

Lasd: [XQL](xql.html), [XPath](XPath.html), [xindice](xindice.html), [tamino](tamino.html), valamint XML alapu [RPC](RPC.html)-k (mert az a tuti-frnko) [XML object mapping](XML%20object%20mapping.html)
