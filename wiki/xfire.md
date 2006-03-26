---
creationDate        : 2005-03-21 11:09:26 +0100 
author              : admin 
title               : xfire 
name                : xfire 
layout              : wiki 
path                : xfire 
date                : 2006-03-26 01:51:28 +0100 
version             : 1 
creator             : kocka 
---
![image](http://xfire.codehaus.org/xfire_logo.jpg)(http://xfire.codehaus.org/)

Egy uj generacios [SOAP](SOAP.html) framework, tobbfele [IoC](ioc.html) integracioval ([picocontainer](picocontainer.html), [loom](loom.html), [spring](spring.html) - errol meg lent!), [JBI](JBI.html)-vel, tobbfele transport layerrel, stb.

Ami igazan erdekes es korszeru benne az az, hogy gyakorlatilag [pojo](pojo.html) alapon programozhatsz, azaz csak csinalsz egy [java](java.html) osztalyt, teljesen hetkoznapi metodusokkal, es egy [xml](XML.html) fileban beregisztralod ezt webservice-kent.

Magyarul [wsdl](WSDL.html)t sem irtal. A [wsdl](WSDL.html)t majd ugy kapod meg hogy elkered a szervertol. Allitolag gyorsabb is, es ebben hajlamos vagyok hinni, de azert meg egy benchmarkot kiprobalok eccer ha lesz idom :)

Azert a hianyossagokrol: szedegetheted ossze magadnak a dependency-ket. Vagy [jaxb](jaxb.html) vagy [xmlbeans](Missing.html) bindingot hasznalsz, ha egyik se tetszik hasznalhatsz dinamikus interfacet amihez meg doko nincsen...

A [spring](spring.html) integracioja egesz erdekes. Nyilvan evidens modon a [spring](spring.html) beaneket felhasznalhatod mint [webservice](Missing.html), ami uber-rulez.

Van egy sajat belso processing pipeline-ja, amit erdemes vegignezni, handlereket assignolhatsz mindenfele feldolgozasi fazishoz, peldaul felhasznalo azonositast is.

Lasd: [webservices](WebServices.html)
