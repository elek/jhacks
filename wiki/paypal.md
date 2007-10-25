---
creationDate        : 2007-10-25 15:23:01 +0200 
author              : kocka 
title               : paypal 
name                : paypal 
layout              : wiki 
path                : paypal 
date                : 2007-10-25 15:23:34 +0200 
version             : 2 
creator             : kocka 
---
[http://www.paypal.com/](http://www.paypal.com/)

[http://developer.paypal.com/](http://developer.paypal.com/)

A világ egyik vezető webes payment szolgáltatója. Egy-két tapasztalat velük kapcsolatban:

__Kontra__:

*   A [java](java.html) api kicsit gebasz. Jelenleg két verzió van: NVP (ez ilyen sima http requestek) és [SOAP](SOAP.html). Az NVP az kétségtelenül működőképesebb, viszont kb mintha Properties objektumokat manipulálnál, na olyan. A SOAP apin viszont sajnos nincsenek meg ugyanazok a hívások és attribútumok.
*   Dokumentáció: elég rendesen szétszórva, sajnos ami van az elég híg, inkáb fórumokbn érdemes bogarászni
*   A sandbox sajnos naponta 3-4 órát pihen, de van úgy hogy több napig sem elérhető, ilyenkor a [SOAP](SOAP.html) kliensed [XML](XML.html) parsolási hibákat vág hozzád például, addig találj magadnak valami más tennivalót (nem, nem másik állást :-D )
*   A support pszichológusok nagyon rendes srácok, de sajnos nincs túl sok idejük az ügyfélre


__Pro__:

*   Úgy is muszáj.
*   Ha a valaki írna hozzá egy pár workaroundot meg egy tisztességes klienst, akkor nagyon egyszerű lenne, de tényleg.


