---
creationDate        : 2006-02-15 23:40:05 +0100 
author              : kocka 
title               : java 1.7/native xml support 
name                : java 1.7/native xml support 
layout              : wiki 
path                : java 1.7/native xml support 
date                : 2006-10-18 13:11:57 +0200 
version             : 4 
creator             : kocka 
---
Egy uj feature a [java 1.7](../java%201.7.html)ben, ami a [java 1.5](../java%201.5.html) [annotations](../annotations.html) ujitasat hasznalja arra hogy egy mappinget nyujtson [XML](../XML.html) es beanek kozott. Vajon minek ilyet egy nyelv magjaba epiteni?

Regi elv az hogy az adatreprezentaciot kulonitsuk el a programlogikatol, es nem egy rossz otlet, ez a megoldas amolyan soft link a ketto kozott. A Bean ismeri a sajat reprezentaciojat.

Mire nem kellene ezt a dolgot hasznalni:

*   Az [XML](../XML.html) adatbazisok egy nagy adag szivas, az [XQL](../xql.html) is tobbnyire alulrol kozeliti az [SQL](../SQL.html) lehetosegeit. Szoval adatbazisokhoz, nagyobb meretu adattarolashoz NEEEE!!!

Mire lehetne talan hasznalni:

*   Konfiguracios objektumok? (csak kerdezem, meg nem talaltam ki mire lesz jo)

Cikkek:

*   [Native XML support in Dolphin ](http://weblogs.java.net/blog/kirillcool/archive/2005/07/native_xml_supp.html)

Lasd meg: [castor](../castor.html), [xstream](../xstream.html), [jdom](../jdom.html), [dom4j](../dom4j.html), satobbi
