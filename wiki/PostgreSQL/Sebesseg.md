---
creationDate: 1112083219397 
author: kocka 
contentAuthor: kocka 
title: Sebesseg 
contentUpdateDate: 1112083219397 
name: PostgreSQLSebesseg 
layout: wiki 
date: 1112083219397 
creator: kocka 
---
Ilyenkor mindig osszehasonlitgatas szokott jonni mas RDBMS-sekkel, foleg [MySQL](MySQL.html)lel. Egyszeru lekerdezesek eseten a sebessege elfogadhato, bar a mysql alatt van, osszetett lekerdezesek eseten tobbnyire gyorsabb, ha megfeleloen be van hangolva persze. Eleg jo az index kezeles es a query planer, az uj tablespace feature-vel a diszk hasznalat is javul, ezen kivul van egy teljesen uj bgwriter processz is ami a tranzakciosebesseggel tesz majd csodakat varhatoan.

# Tuningolas

Ha egy [SQL](SQL.html) statemented nem megfelelo teljesitmennyel fut, akkor az elso lepes mindig az 'explain' hasznalata, ez egy plan tree-t pakol ki, amibol ertheted hogy a PostgreSQL valojaban milyen muveleteket hajt vegre. A plan tree alapjan donthetsz uj indexek felvetelerol vagy a query attervezeserol.
