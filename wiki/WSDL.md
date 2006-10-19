---
creationDate        : 2005-11-25 15:12:14 +0100 
author              : karenin 
title               : Web service description language 
name                : WSDL 
layout              : wiki 
path                : WSDL 
date                : 2006-10-20 00:34:44 +0200 
version             : 3 
creator             : kocka 
---
Egy [xml](XML.html) nyelv a [webservices](WebServices.html) leirasara. [w3c](w3c.html) specifikacio: [http://www.w3.org/TR/2001/NOTE-wsdl-20010315](http://www.w3.org/TR/2001/NOTE-wsdl-20010315)

Kivalloan alkalmas a dolog rendszerek integraciojara (foleg kulonbozo cegek szolgaltatasai eseteben, vagy kulonbozo platformok ([.net](.net.html) vs [java](java.html)))

Áll egy absztrakt (portType, operation, message, part) és egy konkrét részből (service, port) a kettőt köti össze a binding. A WSDL nem kényszerít technológiát, a hagyomány [WebServices](WebServices.html) esetén pl. mindenféle [SOAP](SOAP.html)-os névterek kerülnek a bidingba, amik megmondják, hogy az absztraktul leírt portType-ok hogy lesznek meghívhatóak.


Lasd: [soap](SOAP.html), [webservices](WebServices.html)
