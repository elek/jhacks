---
creationDate: 1108564240401 
author: kocka 
contentAuthor: kocka 
title: PL-J/JDBC 
contentUpdateDate: 1108565832022 
name: PL-JJDBC 
layout: wiki 
date: 1108565832022 
creator: kocka 
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
