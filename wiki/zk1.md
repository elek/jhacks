---
creationDate        : 2006-10-31 22:26:12 +0100 
author              : karenin 
title               : zk1 
name                : zk1 
layout              : wiki 
path                : zk1 
date                : 2007-05-29 15:59:35 +0200 
version             : 2 
creator             : karenin 
---
[zk1](http://zk1.sourceforge.net/)

Ügyes [ajax](ajax.html) framework javahoz. Lényege, hogy egy XUL-ra épülő XML szintakszissal lehet a komponenseket megadni, amikben lehet pure Java-t is használni. Kimenetkor egy saját dispatcher servlet meghíváskor átfordítja HTML-é a definíciót. Egy másik szerveren keresztül pedig intézi az aszinkron kommunikációt, (amiből mi nem látunk semmit, csak azt, hogy regisztrálni kell a servletet)

Szimpatikusnak tűnhet mert:

*   úgy használhatunk ajaxos megoldásokat, hogy mindent Javaban (+XML) írunk le
*   nagyon tisztességesen ledokumentált
*   elég bő alap komponens-e [készlete](http://www.zkoss.org/zkdemo/userguide/) van.

Auth Gábor [előadása](http://jum.anzix.hu/pages/viewpage.action?pageId=557065) szerint fentartásokkal kell kezelni: nagyon alul van dokumentálva, debugolni nagyon nehéz, és a gyakorlatilag pure Java-nak megfelelő szkript nyelvén írt szkriptek pont nem Java fájlokba kerülnek, ezért az IDE támogatással is probélma lehet.
