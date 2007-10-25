---
creationDate        : 2005-03-21 11:10:44 +0100 
author              : kocka 
title               : Simple Object Access Protocol 
name                : SOAP 
layout              : wiki 
path                : SOAP 
date                : 2007-10-25 15:23:56 +0200 
version             : 5 
creator             : kocka 
---
[http://www.w3.org/TR/soap/](http://www.w3.org/TR/soap/)

Ahogy a neve is mutatja objektumok XML-en keresztül való utaztatására mond meg dolgokat. 

Gyakorlatilag egy XML formátum, egy Envelope tegen belül egy Header és egy Body elem képezi a fő részét. A Body-ba gyakorlatilag bármilyen dolgokat tehetünk, a SOAP csak azt mondja meg, hogy a hibát hogyan küldjök vissza, illetve ajánl egy kódolást objektum referenciák jelölésére.

Alapvetően protokol független, mivel a header cuccokat nem a protokol (pl. HTTP) fejlécébe rakja, hanem a saját header-jébe. Ennek előnye, hogy pl. Email-ben is lehet SOAP-ot küldeni, hátránya, hogy a HTTP headerjeit nem használja, ezért újra fel kell találni pl. a session-t és a securityt.


[open source](Open%20Source.html) implementaciok:

*   [xfire](xfire.html) ([codehaus](codehaus.html))
*   [axis](axis.html) ([asf](ASF.html))

java apik:

*   JAX-RPC (maga szint)
*   SAAJ (alacsony szint)

Meg mindenfele kommersz cegnek van nyilvan sajatja, neha a fenti kettore alapozva, neha nem...

Lasd: [WebServices](WebServices.html)


