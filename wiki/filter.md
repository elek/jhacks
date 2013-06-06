---
creationDate        : 2006-01-05 11:58:34 +0100 
author              : admin 
title               : filter 
name                : filter 
layout              : wiki 
path                : filter 
date                : 2006-03-26 01:47:56 +0100 
version             : 1 
creator             : kocka 
---
A filter egy olyan ojjektum, amit ramappelhetsz URL-ekre a [webapp](webapp.html)ban, es a filter objektumodat mindig meghivja az [servlet container](servlet%20container.html) amikor arra az URL-re erkezik keres. Meg azelott hogy meghivodna maga a kiszolgalo [servlet](servlet.html), vagy [jsp](JSP.html). 

Pl egy egyszeru felallas lehet az hogy irsz egy filtert [hibernate](Hibernate.html)hez ami kiszolgalas elott nyit egy hibernate session-t, utanna pedig lezarja.  Ami uber-rulez abbol a szempontbol hogy akkor is le lesz zarva ha a servlet elfelejti :)
