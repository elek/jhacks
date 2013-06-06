---
creationDate        : 2005-02-16 15:47:38 +0100 
author              : admin 
title               : JDBC/takolasok/Orakulum + weblogic 8.1 
name                : JDBC/takolasok/Orakulum + weblogic 8.1 
layout              : wiki 
path                : JDBC/takolasok/Orakulum + weblogic 8.1 
date                : 2006-03-26 01:42:42 +0100 
version             : 1 
creator             : kocka 
---
A [weblogic](../../weblogic.html) 8.1 SP2 altal szolgaltatott [Oracle](../../Oracle.html) driver erdekessegei a kovetkezoek. Tarolt eljarast, ha egy kurzort ad vissza igy kell hivni:<br/>```
pCon.prepareCall("{call pkg_get_resultset.get_rs(?, ?, ?, ?)}");```<br/> es nem igy:<br/> ```pCon.prepareCall("{? = call pkg_get_resultset.get_rs(?, ?, ?, ?)}");```<br/> Kulonben hibat ad vissza.<br/>
A masik erdekesseg, hogy a ResultSet-ben az oszlopok szama nem lehet tobb mint 66, mert kulonben hibat ad a JDBC driver...

([zsoltk](../../zsoltk.html))
