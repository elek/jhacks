---
creationDate        : 2005-02-16 15:50:12 +0100 
author              : admin 
title               : JDBC/takolasok/ResultSetMetaData 
name                : JDBC/takolasok/ResultSetMetaData 
layout              : wiki 
path                : JDBC/takolasok/ResultSetMetaData 
date                : 2006-03-26 01:42:42 +0100 
version             : 1 
creator             : kocka 
---
A kulonbozo JDBC driverek nem tudjak helyesen osszelalitani a [java.sql.ResultSetMetaData](http://docs.oracle.com/javase/7/docs/api/java/sql/ResultSetMetaData.html) objektumot. Ez odaig is fakadhat akar, hogy egy batran kiadott _SELECT * FROM tabla_ utasitas eredmenysorait nem tudod normalisan kiolvasni. Mindegy, hogy indexet vagy nevet hasznalsz, nem lehetsz biztos abban melyik sort is fogod visszakapni. Ezt fontos eszben tartani akkor, amikor valamilyen reflection jellegu dologgal szeretned egy objektum property-jeit beallitani az adatbazisbol.

([zsoltk](../../zsoltk.html))
