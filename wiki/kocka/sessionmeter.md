---
creationDate: 1220395337273 
author: kocka 
contentAuthor: kocka 
title: Sessionmeter 
contentUpdateDate: 1221770361345 
name: kockasessionmeter 
layout: wiki 
date: 1221770361345 
creator: kocka 
---
Egy filter arra, hogy nyomon tudd kovetni a session-od valtozasait.

Ilyesmi lesz a kimenete:
{% highlight java %}
Request: /testapp/index.jsp
Request: /testapp/login.do
- user         NEW 42
Request: /testapp/profile.jsp
- user         NOP 42
Request: /testapp/updateprofile.do
- user         CHG 90
Request: /testapp/logout.do
- user         DEL 42
{% endhighlight %}

__Fontos korlat__: Ez a filter nem ugyanazt meri, mint amit a servlet container-ed. A servlet container-ed minden alkalommal ujra fogja szinkronizalni az adott bean-t, amikor ujra odadobod neki, a filter pedig csak azt tudja nezni hogy a kiserializalt minta valtozott-e. Van olyan eset, amikor nem jelez kapast, pedig a servlet container ujraszinkronizalja a dolgot. Feltetelezzuk hogy nem csinal teljesen hiabavalo munkat az alkalmazasod :)

Es az egeszet ide irtam le: http://iwillworkforfood.blogspot.com/2008/09/sessionmeter.html
