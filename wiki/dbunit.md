---
creationDate        : 2006-06-22 00:01:43 +0200 
author              : kocka 
title               : dbunit 
name                : dbunit 
layout              : wiki 
path                : dbunit 
date                : 2006-06-22 00:01:43 +0200 
version             : 1 
creator             : kocka 
---
Egy kis [junit](junit.html)-kozeli library, ami olyanokra jo mint kis tesztadatbazisok inicializacioja integracios vagy [dao](DAO.html) tesztekhez.

Junit 3.x felhasznalok egyszeruen extendelhetik a sajat kis testcase-leszarmazottjat, vagy ha ennel van jobb otlet is, akkor par api hivassal a setUp-ban is megoldhato siman.

Az adatokat valtozatos formaban lehet tarolni, [csv](Missing.html), [xml](XML.html) formatumok...

Ami szopacs volt benne nekem, az az hogy [hibernate](Hibernate.html)-vel hogy bekitsem ossze de egy apro architekturalis hegesztessel sikerult.
