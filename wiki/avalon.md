---
creationDate        : 2004-07-26 15:44:08 +0200 
author              : kocka 
title               : avalon 
name                : avalon 
layout              : wiki 
path                : avalon 
date                : 2006-02-28 14:37:41 +0100 
version             : 13 
creator             : kocka 
---

Szoval reges regen letezett egy avalon project az [ASF](ASF.html)nel [http://avalon.apache.org](http://avalon.apache.org) cimen. Ezt feloszlattak, mert teljesen mozgaskeptelen volt. Ennek ellenere az avalon framework el, es van aki karbantartsa.


Az avalon orokosei:

*   [http://excalibur.apache.org/](http://excalibur.apache.org/) framework karbantartas, komponensek
*   [http://www.dpml.net/](http://www.dpml.net/) ide jott a hajbakapott avalon csapat es a merlin tobbek kozt
*   [loom](loom.html) a korabban elkoltozott csapat a phoenix utodjaval.


Az Avalon egy komponens framework. Segitsegevel az alkalmazasunkat ujrefalhsznalhato komponensekbol epithetjuk. (lasd meg [COP](COP.html), [IoC](ioc.html))
Az avalon egy hatranya, hogy ahhoz hogy avalon containerben mukodjon a komponensed, ahhoz implementalnod kell tucat [lifecycle](lifecycle.html) interfacet, ami avalon fuggove teheti a komponensedet. (a konfiguaciot es a dependency-ket is beleertve)
A megoldas: vagy wrappeld, vagy extendeld egy avalon fuggo osztallyal a fuggetlen osztalyodat. Ezzel csak az a bajom, hogy a komponensek tipikusan nagyon kicsi kodot tartalmaznak, most implementalni egy ilyen osztalyt avalonhoz es [picocontainer](picocontainer.html)hez es [spring](spring.html)hez, es ott tartassz hogy a wrapper kod haromszor akkora mint a tulajdonkeppeni komponens.
Az avalon viszont az elsok kozott volt, es ar van hozza mindenfele implementacio, a kis beagyazott kornyezetektol ([plexus](plexus.html)) a szerver oldaliig ([loom](loom.html)) minden. Szoval kulonosebben nem lesz attol kornyezetfuggo az alkalmazasod mert avalon-ra kodoltad ra. (na ezek inkab a [PL-J](PL-J.html)vel kapcsolatos gondolataim voltak :)

Az avalon project 3 lenyeges resze:

1.   framework [http://ashkelon.forgeahead.hu/api.main.do?id=107](http://ashkelon.forgeahead.hu/api.main.do?id=107)
1.   components
1.   containers

A __framework__ tartalmazza az interface-ket, amiket implementahlatunk es hasznalhatunk komponenseinkkel.

A __components__ egy tucatnyi mar elore megirt komponens konyvtara.

Container-bol jelenleg tobb is van:

1.   Merlin: az avalon csapat jelenlegi implementacioja. Architekturalisan nagyon baba, sajnos se nem tul stabil eddig se nem tul managelheto, de azert jo...
1.   Phoenix, @deprecated :( sajnos, pedig nagyon szerettem. JMX extension
1.   [Loom](loom.html). A phoenix utodja. Architekturalis atberhelesek, szerver oldalra eleg jo. Megy vele minden ami a phoenixben ment. [http://loom.codehaus.org](http://loom.codehaus.org)
1.   [Plexus](plexus.html). Light weigth container, beagyazhato. [http://plexus.codehaus.org](http://plexus.codehaus.org)

Avalonra epulo alkalmazasok:

1.   [james](james.html) (java mail server) [http://james.apache.org](http://james.apache.org)
1.   [cocoon](cocoon.html) [http://cocoon.apache.org](http://cocoon.apache.org)
1.   telnetd, [ftpserver](ftpserver.html), etc [http://incubator.apache.org](http://incubator.apache.org)
1.   [KLEEN](KLEEN.html)
1.   [java jabber server](java%20jabber%20server.html)
1.   es persze a vilaghiru [PL-J](PL-J.html) es [harvest](harvest.html) szoftverek :)


