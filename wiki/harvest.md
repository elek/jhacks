---
creationDate        : 2004-07-26 13:01:08 +0200 
author              : kocka 
title               : harvest 
name                : harvest 
layout              : wiki 
path                : harvest 
date                : 2005-03-07 13:58:33 +0100 
version             : 10 
creator             : kocka 
---

-   [harvest/containers](harvest/containers.html)
-   [harvest](harvest.html)




A Harvest egy java alapu rugalmas alkalmazas integracios megoldas. Java komponensek gyujtemenye, amibol barki osszeallithatja -esetleg sajat kiegeszitessel- a sajat sszuksegleteinek megfelelo cuccot.


Sajnos kicsit tul altalanos ahhoz hogy meg tudjam fogalmazni hogy pontosan mi is. Igazabol tobbfele rendszernek kepezheti alapjat.
A sajat 5leteim:

1.   replikacios megoldas \(cross-db, cross-db-structure\)
1.   [ETL](ETL.html) eszkoz \(extraction transformation load\)
1.   rendszer integracios platform \(szinkron, asszinkorn\)

Jelenleg [Tyrex](tyrex.html)-et tartalmaz tranzakcio kontrollerkent, [j2ee](j2ee.html) kornyezet integracio folyamatban.

A jovoben a [PL-J](PL-J.html)-vel integralva szeretnek egy kemeny integracios megoldast fejleszteni belole.

A harvest tipikus komponensei:

*   source: az az objektum ami eleri a valodi adatforrast es objektumokat csinal hoz el onnet (ha esetleg nem egybol objektumok lennenek ott is)
*   filter: a filter megkapja az objektumokat amiket a source betoltott, es vissza kell adnia objektumokat. A ketto kozott akarmi lehet, a bean-ek tulajdonsagait felulirhatja, mas benaekkel helyettesitheti oket, vagy ki is dobhatja mindet.
*   persister: egy tarba perzisztalja az kapott beaneket. Tipikus megoldas lehet egy SQL adatbazis.
*   tranzakcio vezerlo: aki a tranzakciot vezerli [TM](Missing.html).
*   asszinkron beantolto: tartalmazza a logikat ami az idoziteshez, a bean forras, a filterek es a persister es a tranzakcio kezelesehez szukseges. Neki nincs interface, mert ugy sem akarja senki sem piszkalni, legfeljebb lesz majd egy MBean-je ([JMX](JMX.html)).
