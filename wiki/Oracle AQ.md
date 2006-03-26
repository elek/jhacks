---
creationDate        : 2005-10-19 16:18:27 +0200 
author              : admin 
title               : Oracle Advanced Queueing 
name                : Oracle AQ 
layout              : wiki 
path                : Oracle AQ 
date                : 2006-03-26 01:42:49 +0100 
version             : 1 
creator             : kocka 
---
Egy [MOM](MOM.html) az [Oracle](Oracle.html) [RDBMS](RDBMS.html) termekbe epitve, gyakorlatilag egy tucat PL/SQL eljarasbol megepitve. Egy sajatos, [JMS](JMS.html)-t is implementalo [java](java.html) APIn keresztul lehet elerni, persze csak a standard feature-ket, a tobbit [Oracle](Oracle.html) specifikus APIn keresztul.

nehany erdekesseg/tapasztalat:

*   Az AQ sajat [jms](JMS.html) extensionjaval meg tudod azt oldani hogy az egy tranzakcioban bekommitolt uzeneteket egy csoportkent szeded ki. Jol hangzik mi? :) Persze ehhez valami falabu API-t irtak a oracle sracok, de mukodik.
*   Nyilvan PL/SQL bol is tudsz messageket betolteni, igy pl egy idiota autokommitos tranzakcios webappot is tulelhet az appod. Mar ha tul lehet elni ekkora marhasagot :)
*   Nem egy JMS szerver, hanem egy standalone, Oracle specifikus dolgokkal peldanyosithato JMS api ami az adatbazishoz fer hozza (igen, peldanyositashoz kell egy [JDBC](JDBC.html) kapcsolat). Ennek kovetkezteben az [alkalmazas szerver](Alkalmazas%20Szerver.html) integraciot csinald magad modon :( [weblogic](weblogic.html)hoz van egy adapter de inkab ne is lenne, szoval mondhatni hogy [oc4j](oc4j.html)n kivul semmi nem mukodik egyut vele, leszamitva olyan dolgokat mint [mule](mule.html). (dehat a [mule](mule.html) mindennel)

Amugy mokas kis cucc, meg jo lassu :) Az Oracle 9i ota minden adatbazisban benne van. Egy ilyet igazabol nem lenne nagy kunszt megirni [PostgreSQL](PostgreSQL.html)re sem.
