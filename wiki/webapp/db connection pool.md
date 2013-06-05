---
creationDate: 1112043823603 
author: kocka 
contentAuthor: kocka 
title: webapp/db connection pool 
contentUpdateDate: 1190214009129 
name: webappdb connection pool 
layout: wiki 
date: 1190214009129 
creator: kocka 
---
Na megis, azoknak, akik sajat connection poolt integralnak a [webapp](../webapp.html)jaikba.

*   Connection pool mar letezik, ilyen peldaul a [commons](../commons.html)-dbcp.
*   De viszont meg csak ezt sem kell integralni a [webapp](../webapp.html)ba.
*   Hanem [JNDI](../JNDI.html)n keresztul lookupolni kell egy ot, es attol kerni egy -t. Aztan amikor mar nem kell akkor bezarni. (standard [j2ee](../j2ee.html) megoldás)
*   Esetleg [spring](../spring.html)-re bizni a dolgot es nem foglalkozni a dologgal. (modernebb [ioc](../ioc.html) megoldás)
