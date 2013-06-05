---
creationDate: 1108117669962 
author: kocka 
contentAuthor: kocka 
title: JCache 
contentUpdateDate: 1165830636088 
name: JCache 
layout: wiki 
date: 1165830636088 
creator: kocka 
---
[Java](java.html) cache specifikacio, [jsr 107](http://www.jcp.org/en/jsr/detail?id=107)
Dokumentumokat egyelore csak [itt](https://jsr-107-interest.dev.java.net/) lehet elerni, mivel nincsen public release, meg itt van egy jar hogy lasd hogy fog kinezni: http://www.ibiblio.org/maven/jcache/jars/jcache-1.0-dev-2.jar (referencia implementacioval)

A moka az hogy  leszarmazott a javax.cache.Cache osztaly, ugyhogy egyszeruen egy mapkent fersz hozza. Es ebbol persze van tranzakcionalis, tavoli, clusterezett, pirospottyos, meg mindenfele.

__[Kocka](kocka.html) says__: Nyugodtan kossetek bele ebbe, de szerintem architekturat cache-re epiteni nem egy siraj otlet. Egyszerubb egy normalis [persistence](persistence.html) rendszerre epiteni es az alatt legyen a cache, szoval elmeletileg egy [j2ee](j2ee.html) alkalmazas fejlesztonek nem kellene tudnia a cache kezelesrol, csak a perzisztencia letezeserol. Lasd: [hibernate](Hibernate.html), [jdo](JDO.html), egyeb [or mapping](OR%20Mapping.html)

Lasd meg: [coherence](coherence.html), [javaspace](Missing.html), [fcache](FCache.html), [activespace](ActiveSpace.html), [oscache](oscache.html) stb...


