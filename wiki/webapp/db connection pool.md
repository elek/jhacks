---
creationDate        : 2005-03-28 23:03:43 +0200 
author              : kocka 
title               : webapp/db connection pool 
name                : webapp/db connection pool 
layout              : wiki 
path                : webapp/db connection pool 
date                : 2007-09-19 16:59:52 +0200 
version             : 2 
creator             : kocka 
---
Na megis, azoknak, akik sajat connection poolt integralnak a [webapp](../webapp.html)jaikba.

*   Connection pool mar letezik, ilyen peldaul a [commons](../commons.html)-dbcp.
*   De viszont meg csak ezt sem kell integralni a [webapp](../webapp.html)ba.
*   Hanem [JNDI](../JNDI.html)n keresztul lookupolni kell egy [javax.sql.DataSource](http://docs.oracle.com/javase/7/docs/api/javax/sql/DataSource.html)ot, es attol kerni egy [java.sql.Connection](http://docs.oracle.com/javase/7/docs/api/java/sql/Connection.html)-t. Aztan amikor mar nem kell akkor bezarni. (standard [j2ee](../j2ee.html) megoldás)
*   Esetleg [spring](../spring.html)-re bizni a dolgot es nem foglalkozni a dologgal. [modernebb [ioc](../Missing.html) megoldás]
