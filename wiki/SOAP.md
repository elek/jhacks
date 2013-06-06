---
creationDate        : 2005-03-21 11:10:44 +0100 
author              : kocka 
title               : Simple Object Access Protocol 
name                : SOAP 
layout              : wiki 
path                : SOAP 
date                : 2007-10-25 16:06:31 +0200 
version             : 7 
creator             : kocka 
---
[http://www.w3.org/TR/soap/](http://www.w3.org/TR/soap/)

Ahogy a neve is mutatja objektumok [XML](XML.html)-en keresztül való utaztatására mond meg dolgokat. 

Gyakorlatilag egy [XML](XML.html) formátum, egy Envelope tegen belül egy Header és egy Body elem képezi a fő részét. A Body-ba gyakorlatilag bármilyen dolgokat tehetünk, a SOAP csak azt mondja meg, hogy a hibát hogyan küldjök vissza, illetve ajánl egy kódolást objektum referenciák jelölésére.

Alapvetően protokol független, mivel a header cuccokat nem a protokol (pl. HTTP) fejlécébe rakja, hanem a saját header-jébe. Ennek előnye, hogy pl. Email-ben is lehet SOAP-ot küldeni, hátránya, hogy a [HTTP](HTTP.html) headerjeit nem használja, ezért újra fel kell találni pl. a session-t és a securityt.


[open source](Open%20Source.html) implementaciok:

*   [xfire](xfire.html) ([codehaus](codehaus.html))
*   [cxf](cxf.html) ([asf](ASF.html))
*   [axis](axis.html) ([asf](ASF.html))
*   Meg mindenfele kommersz cegnek van nyilvan sajatja

java apik:

*   JAX-RPC (magas szint)
*   SAAJ (alacsony szint)

Lasd: [WebServices](WebServices.html)


