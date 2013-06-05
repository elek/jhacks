---
creationDate: 1194611331425 
author: kocka 
contentAuthor: kocka 
title: Kicsi horror 
contentUpdateDate: 1194611331425 
name: WTFMSSQL cluster 
layout: wiki 
date: 1194611331425 
creator: kocka 
---
Hozzávalók: 

*   [MSSQL](MSSQL.html) ('cluster') (azt hiszem a 1998-as kiadás, szóval nem mai darab)
*   egy már létező view
*   kis balszerencse



Elkészítés: futtasd le az adatbázis szerveren egy update scriptet (ezt nem tudom meghatározni, hogy milyen kritériumok alapján kell elkészíteni)

## Az eredmény


A view-en végrehajtott select eredményhalmazában az adatok egy oszloppal balra tolódnak el. Az oszlopok nem, csak az adatok. Például egy olyan oszlopban, ahol számot kérdeztél, simán lesz string, az [mssqlt](MSSQL.html) nem fogja érdekelni.

## Ha meguntad a mókát


Droppold le a view-t, hozd létre újra, az eredmény most -remélhetőleg- jó lesz.
