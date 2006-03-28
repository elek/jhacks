---
creationDate        : 2005-03-28 23:37:36 +0200 
author              : kocka 
title               : Content repository 
name                : Content repository 
layout              : wiki 
path                : Content repository 
date                : 2006-03-28 15:32:31 +0200 
version             : 18 
creator             : kocka 
---
Tartalom kezelő rendszer - magyarul. Leginkab ugy nez ki mint egy [XML](XML.html) adatbazis, de talan azert nem annyira rossz :) Az adatokat egyszeru [XML](XML.html) szeru faban tarthatod, lekerdezhetsz [xpath](XPath.html) vagy [sql](SQL.html)-szeru nyelven.

[http://www.jcp.org/en/jsr/detail?id=170](http://www.jcp.org/en/jsr/detail?id=170)

Implementaciok:

*   [Jackrabbit](http://incubator.apache.org/jackrabbit/) 
*   [eXo Platform](http://www.exoplatform.org) - Portlet Container, JCR, CMS, minden egyben.
*   [alfresco](http://www.alfresco.org/)

penzes cuccos:

*   documentum, elterjedt de nagyon furi dolgok vannak benne. Pl ahogy kliens webappot kellett hozza fabrikalni, az enyhen szolva [gyanus](gyanus.html). Az ararol meg legendak keringenek.

Cikkek:

*   [Introducing the Java Content Repository API](http://www-128.ibm.com/developerworks/java/library/j-jcr/)
*   [Catch Jackrabbit and the Java Content Repository API](http://www.artima.com/lejava/articles/contentrepository.html)

[cms](CMS.html)ek amik tamogatjak a szabvanyt:

*   [http://www.magnolia.info](http://www.magnolia.info) ([lgpl](LGPL.html))

Erdekes lehet meg: peldaul a [cocoon](cocoon.html) is tamogatja a CR-t mint tartalom forrast, sajat kis adapteren keresztul. Egy megfelelo konfig, egy kis [xslt](XSLT.html) es egesz jo kis prezentacios rendszert kaphatsz...

Lasd meg: [XML](XML.html), [CMS](CMS.html), esetleg [portlet](portlet.html)
