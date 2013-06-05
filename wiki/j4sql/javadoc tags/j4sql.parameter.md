---
creationDate: 1114190593262 
author: kocka 
contentAuthor: kocka 
title: j4sql/javadoc tags/j4sql.parameter 
contentUpdateDate: 1120165427015 
name: j4sqljavadoc tagsj4sql.parameter 
layout: wiki 
date: 1120165427015 
creator: kocka 
---
Egy parameter leirasat lehet vele meghatarozni [j4sql/javadoc tags/j4sql.function](../../j4sql/javadoc%20tags/j4sql.function.html) es [j4sql/javadoc tags/j4sql.procedure](../../j4sql/javadoc%20tags/j4sql.procedure.html) eseteben. Ha nem hasznalod, akkor az adatbazis default typemappingjet hasznalja, es parameter neveket general.

Attributumok:

Attributum|kotelezo|leiras|default
name|igen|A java metodusban az attributum neve|
scope|nem|'in' 'out' vagy 'inout'|'in'
type|nem|Az adatbazis tipus|
sqlName|nem|az adatbazis funkcio parameterenek neve|ugyanaz mint a java parameter neve

