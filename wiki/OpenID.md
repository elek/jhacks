---
creationDate        : 2007-02-26 17:45:07 +0100 
author              : kocka 
title               : OpenID 
name                : OpenID 
layout              : wiki 
path                : OpenID 
date                : 2007-11-30 14:27:57 +0100 
version             : 6 
creator             : karenin 
---
[http://openid.net/](http://openid.net/)

Decentralizál lightweight URL alapú identity megoldás. Gyakorlatilag egy url-lel lépkedhetünk be az oldalakra. Beléptetés helyett az oldal átdob a server identity provider-hez, hogy ő léptessen be, az identity provider meg vissza redirecteli a böngészőt az oldalra a válasszal, hogy sikerült-e.

Az OpenID Attribute Exchange kiterjesztéssel közben el lehet kunyerálni a provider-től alap adatokat is (email, születési év, stb.) Persze az identity provider általában megkérdezi a usert, hogy tényleg kiadhatja-e az adatokat.

Lásd még: 

*   [Acegi](acegi.html) (sandbox-ban)

Linkek:

*   [Neltz Tamás előadása a Newtech Meetup-on](http://video.google.com/videoplay?docid=7684630973021077375)
*   [TSS - Using OpenID](http://www.theserverside.com/tt/articles/article.tss?l=OpenID)
*   [OpenId-Server](http://code.google.com/p/openid-server/) [java](java.html) [webapp](webapp.html) implementáció
