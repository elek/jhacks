---
creationDate        : 2004-12-28 23:18:34 +0100 
author              : kocka 
title               : PL-J/Java Tarolt Eljarasok 
name                : PL-J/Java Tarolt Eljarasok 
layout              : wiki 
path                : PL-J/Java Tarolt Eljarasok 
date                : 2004-12-28 23:18:34 +0100 
version             : 1 
creator             : kocka 
---
Szoval miert is jo az hogy az adatbazisban is hajthatunk java kodot? Sok okot lehet felhozni.

*   Tarolt eljarasok, UDF-ek es triggerek vegrehajtasara egyszeruen szuksegunk van, vajon akarunk-e ehhez meg egy nyelvet megtanulni? (mint pl PLSQL, transact sql, meg ilzesmik) Az nyilvanvalo hogy egy PLSQL kod sokkal kompaktabban fejezi ki a lenyeget mint a java kod, ha adatbazishozzaferesrol beszelunk. A PLSQL viszont nehezen portolhato, kevesen ismerik, es olyan franko [ide](../IDE.html) sincs hozza mint az [eclipse](../Eclipse.html) :)
*   Hogy lassabb-e a Java mint a PLSQL? Jelenleg igen, az [oracle](../Oracle.html) implementaciojaban mindenkeppen, a [Postgresql](../PostgreSQL.html) implementaciojaban meg szinten, de ez nem lesz sokaig igy.
*   Kod duplikacio kiiktatasa. ugyanazzal a koddal amivel ellenorzol a java processzeidben, ellenorizhetsz az adatbazisban is.

A [PL-J](../PL-J.html) az az [RDBMS](../RDBMS.html)ed szamara mint ami a [mod_jk](../mod_jk.html) es a [Tomcat](../tomcat.html) a [httpd](../httpd.html) szamara. Egy eszkoz ahol biztonsagban futtathato felhasznalo altal irt kod.
