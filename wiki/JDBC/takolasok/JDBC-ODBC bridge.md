---
creationDate: 1108565169761 
author: kocka 
contentAuthor: kocka 
title: JDBC/takolasok/JDBC-ODBC bridge 
contentUpdateDate: 1108565169761 
name: JDBCtakolasokJDBC-ODBC bridge 
layout: wiki 
date: 1108565169761 
creator: kocka 
---
A JDBC-ODBC Bridge egy rakas szerencsetlenseg, ha csak egy mod van ra ne hasznaljatok! ([Kocka](../../kocka.html), [Sybase](../../Sybase.html)-zel)

Resultset olvasas mindig csak a kovetkezokeppen: balrol jobbra, fentrol lefele, mintha konyvet olvasnal. Azaz ha elobb a 2., majd az 1. oszlopot olvasod, egy furcsa JDBCExceptiont kapsz az arcodba :(
