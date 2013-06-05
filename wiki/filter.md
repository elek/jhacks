---
creationDate: 1136458714070 
author: kocka 
contentAuthor: kocka 
title: filter 
contentUpdateDate: 1136458714070 
name: filter 
layout: wiki 
date: 1136458714070 
creator: kocka 
---
A filter egy olyan ojjektum, amit ramappelhetsz URL-ekre a [webapp](webapp.html)ban, es a filter objektumodat mindig meghivja az [servlet container](servlet%20container.html) amikor arra az URL-re erkezik keres. Meg azelott hogy meghivodna maga a kiszolgalo [servlet](servlet.html), vagy [jsp](JSP.html). 

Pl egy egyszeru felallas lehet az hogy irsz egy filtert [hibernate](Hibernate.html)hez ami kiszolgalas elott nyit egy hibernate session-t, utanna pedig lezarja.  Ami uber-rulez abbol a szempontbol hogy akkor is le lesz zarva ha a servlet elfelejti :)
