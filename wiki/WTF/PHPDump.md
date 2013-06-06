---
creationDate        : 2005-05-25 13:45:29 +0200 
author              : admin 
title               : WTF/PHPDump 
name                : WTF/PHPDump 
layout              : wiki 
path                : WTF/PHPDump 
date                : 2006-03-26 01:43:02 +0100 
version             : 1 
creator             : kocka 
---
Ez egy mispattern inkab mint [java](../java.html) specifikus agymenes.

A kovetkezot kell tenned: ahelyett hogy DB dumpot vagy db fuggetlen xml-t dumpolnal be az adatbazisba, keszitessz egy [php](../PHP.html) scriptet ami beteszi a cuccodat az adatbazisba, ezt kiteszed akarhova a weboldaladra es meghivod. Ezt legelosszor egy [php](../PHP.html) programozotol lattam, es ha nem ult volna kozvetlenul mellettem ott helyben bekuldtem volna a szanalmas.hu-ra is :-D

A gebasz az volt mondjuk hogy a [php](../PHP.html) a timeout utan kinyirta a scriptet es igy az adatoknak talan fele ment be. Milyen jok is ezek a tranzakciok :)

Egy hasonlo megoldas mukodik a [snipsnap](../SnipSnap.html)ban is, bar annyi kulonbseg azert van hogy a [snipsnap](../SnipSnap.html) opensource leven valami azonositast is ker a muvelet vegrehajtasahoz. 

Mindenesetre nagyon nem igy kellene csinalni. Nem azert van [javax.sql.DataSource](http://docs.oracle.com/javase/7/docs/api/javax/sql/DataSource.html) hogy mindenki sajat poolt csinaljon, meg [JMX](../JMX.html) hogy mindenki maga managelje.
