---
creationDate        : 2004-09-09 11:53:59 +0200 
author              : kocka 
title               : FOP 
name                : FOP 
layout              : wiki 
path                : FOP 
date                : 2005-12-06 13:34:12 +0100 
version             : 4 
creator             : kocka 
---
[http://jakarta.apache.org/fop/](http://jakarta.apache.org/fop/)

Az [ASF](ASF.html) renderelo rendszere ami az XSL:FO (formating objects) szabvanybol general elvileg barmlyen kimenetet, bar tobbnyire a [PDF](PDF.html) renderelesre hasznaljak. (ugyan mi masra lenne szukseg? :)
Eleve integralva van a jobb frameworkokbe (pl [cocoon](cocoon.html)) es nagyon konnyen integralhato barhova ahova meg nincs, viszont mielott megtenned:

*   Ugye tudod hogy az [XSLT](XSLT.html) transzformaciok lassuak (persze lehet huzni, de az alkalmazaslogikat nem am erre epiteni :) csak a prezentacios logikat esetleg )
*   A FOP-on is lehetne huzni helyenkent eleg evidens dolgokat. (temporary object kezeles)

Riport renderelesre viszont egeszen kivallo, ajanlom mindenkinek. Alternativa: [iText](Missing.html), ami viszont azt hiszem csak [PDF](PDF.html)-et tud es nem FO-bol ha jol tudom, viszont legalab furge, ha ez szamit.

Amiert legszivesebben agyonvernem a fop-ot, az az hogy [avalon](avalon.html) [logging](Logging.html)ot hasznal, ami valoszinuleg az egyetlen oka annak hogy az emberek [avalon](avalon.html) framework jarokat pakolnak a rendszerukbe.
