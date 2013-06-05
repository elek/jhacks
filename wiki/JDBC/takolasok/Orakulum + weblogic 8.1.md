---
creationDate: 1108565258911 
author: kocka 
contentAuthor: kocka 
title: JDBC/takolasok/Orakulum + weblogic 8.1 
contentUpdateDate: 1108565258911 
name: JDBCtakolasokOrakulum + weblogic 8.1 
layout: wiki 
date: 1108565258911 
creator: kocka 
---
A [weblogic](../../weblogic.html) 8.1 SP2 altal szolgaltatott [Oracle](../../Oracle.html) driver erdekessegei a kovetkezoek. Tarolt eljarast, ha egy kurzort ad vissza igy kell hivni:<br/>{% highlight java %}
pCon.prepareCall("\{call pkg_get_resultset.get_rs(?, ?, ?, ?)\}");{% endhighlight %}<br/> es nem igy:<br/> {% highlight java %}pCon.prepareCall("\{? = call pkg_get_resultset.get_rs(?, ?, ?, ?)\}");{% endhighlight %}<br/> Kulonben hibat ad vissza.<br/>
A masik erdekesseg, hogy a ResultSet-ben az oszlopok szama nem lehet tobb mint 66, mert kulonben hibat ad a JDBC driver...

([zsoltk](../../zsoltk.html))
