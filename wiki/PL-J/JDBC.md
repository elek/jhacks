---
creationDate        : 2005-02-16 15:30:40 +0100 
author              : kocka 
title               : PL-J/JDBC 
name                : PL-J/JDBC 
layout              : wiki 
path                : PL-J/JDBC 
date                : 2005-02-16 15:57:12 +0100 
version             : 2 
creator             : kocka 
---
A [PL-J](../PL-J.html) [JDBC](../JDBC.html) drivere. Sajatos allatfaj:

*   Nem nyit TCP kapcsolatot, mert mar letezik.
*   Ha tobb apcsolatot nyitsz, akkor is mind ugyanazon a csatornan keresztul fog menni.
*   tranzakcio kezeles: nincs, de ha lesz, akkor is csak nested tranzakciok.
*   Semmit nem tud a frontend-backend protokolrol, a chanell-ra epul.
*   A RDBMS tipusokrol se tud semmit, a typemapper szolgaltatast hasznalja.
*   Metainformaciok a konfiguraciobol.
*   Erosen konfiguralhato.
*   Plan pool. Az prepared statement-ekhez megtartja egy ideig a plan-t, ezt tobbszor felhasznalhatja.

Hat ennyi, szoval egy atlagos [JDBC](../JDBC.html) drivertol sokban kulonbozik.
