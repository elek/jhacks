---
creationDate        : 2005-02-16 15:46:09 +0100 
author              : admin 
title               : JDBC/takolasok/JDBC-ODBC bridge 
name                : JDBC/takolasok/JDBC-ODBC bridge 
layout              : wiki 
path                : JDBC/takolasok/JDBC-ODBC bridge 
date                : 2006-03-26 01:42:42 +0100 
version             : 1 
creator             : kocka 
---
A JDBC-ODBC Bridge egy rakas szerencsetlenseg, ha csak egy mod van ra ne hasznaljatok! ([Kocka](../../kocka.html), [Sybase](../../Sybase.html)-zel)

Resultset olvasas mindig csak a kovetkezokeppen: balrol jobbra, fentrol lefele, mintha konyvet olvasnal. Azaz ha elobb a 2., majd az 1. oszlopot olvasod, egy furcsa JDBCExceptiont kapsz az arcodba :(
