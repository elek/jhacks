---
creationDate        : 2006-03-12 09:42:49 +0100 
author              : pedro 
title               : eXist 
name                : eXist 
layout              : wiki 
path                : eXist 
date                : 2006-03-12 11:25:47 +0100 
version             : 8 
creator             : pedro 
---
Nyílt forrású natív [XML](XML.html) adatbázis. Natív alatt azt kell érteni, hogy az adattárolás történik [XML](XML.html)-ben.

![image](http://wiki.exist-db.org/space/SnipSnap/config/logo.png)(http://exist.sourceforge.net/)

[eXist - Open Source Native XML Database](http://exist.sourceforge.net/)

Sok mindenre használható ... egyenlőre sajnos komoly hiányosságai vannak.

Lekérdezés és hozzáférés mehet sok formában:

*   [XML:DB](http://xmldb-org.sourceforge.net/) kezdeményezés API-ját használva,
*   [REST](REST%20-%20Representational%20State%20Transfer.html) stílusú HTTP-vel (thanks to [Jetty](jetty.html)),
*   [XML-RPC](xml-rpc.html)-vel,
*   [SOAP](SOAP.html) alapú webszolgáltatásokkal,
*   [WebDAV](Webdav.html)-val ... ez a része nagyon komoly ... sajnos még nem teljes
*   [XQuery](XQuery.html)-vel (majdnem teljes) ... esetleg megtámogatva:
*   [XPath](XPath.html)-tal,
*   dokument és csomópont szintű update [XUpdate](Missing.html)-tel.


Komoly hiányosságok:

*   nincs tranzakció kezelés,
*   nincs schema validálás ... meg egyáltalán schema kezelés,
*   az [XQuery](XQuery.html) támogatás egyenlőre 97%-os ... ráadásul a keménymagos funkciók out of scope.

Ha lib-ként használod, alapból eléred mind az alap, mind az [XQuery](XQuery.html)-vel előállított [XML](XML.html) doksi [DOM](dom.html)-ját. Néhány óra doksi olvasás után be tudtam tolni [JonAS](jonas.html) alá ... onnantól kezdve a web konténerből mindenféle úton-módon lehet használni. [EJB](EJB.html) konténerről egyenlőre ne beszéljünk ... amúgy sincs tranzakciókezelés ...
