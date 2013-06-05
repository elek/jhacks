---
creationDate: 1108565412107 
author: kocka 
contentAuthor: kocka 
title: JDBC/takolasok/ResultSetMetaData 
contentUpdateDate: 1108565412107 
name: JDBCtakolasokResultSetMetaData 
layout: wiki 
date: 1108565412107 
creator: kocka 
---
A kulonbozo JDBC driverek nem tudjak helyesen osszelalitani a  objektumot. Ez odaig is fakadhat akar, hogy egy batran kiadott _SELECT * FROM tabla_ utasitas eredmenysorait nem tudod normalisan kiolvasni. Mindegy, hogy indexet vagy nevet hasznalsz, nem lehetsz biztos abban melyik sort is fogod visszakapni. Ezt fontos eszben tartani akkor, amikor valamilyen reflection jellegu dologgal szeretned egy objektum property-jeit beallitani az adatbazisbol.

([zsoltk](../../zsoltk.html))
