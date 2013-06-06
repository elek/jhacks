---
creationDate        : 2005-04-22 19:23:13 +0200 
author              : admin 
title               : j4sql/javadoc tags/j4sql.parameter 
name                : j4sql/javadoc tags/j4sql.parameter 
layout              : wiki 
path                : j4sql/javadoc tags/j4sql.parameter 
date                : 2006-03-26 01:48:07 +0100 
version             : 1 
creator             : kocka 
---
Egy parameter leirasat lehet vele meghatarozni [j4sql/javadoc tags/j4sql.function](../../j4sql/javadoc%20tags/j4sql.function.html) es [j4sql/javadoc tags/j4sql.procedure](../../j4sql/javadoc%20tags/j4sql.procedure.html) eseteben. Ha nem hasznalod, akkor az adatbazis default typemappingjet hasznalja, es parameter neveket general.

Attributumok:

Attributum|kotelezo|leiras|default
name|igen|A java metodusban az attributum neve|
scope|nem|'in' 'out' vagy 'inout'|'in'
type|nem|Az adatbazis tipus|
sqlName|nem|az adatbazis funkcio parameterenek neve|ugyanaz mint a java parameter neve
