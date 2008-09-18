---
creationDate        : 2008-09-03 00:42:17 +0200 
author              : kocka 
title               : Sessionmeter 
name                : kocka/sessionmeter 
layout              : wiki 
path                : kocka/sessionmeter 
date                : 2008-09-18 22:39:21 +0200 
version             : 10 
creator             : kocka 
---
Egy filter arra, hogy nyomon tudd kovetni a session-od valtozasait.

Ilyesmi lesz a kimenete:
```
Request: /testapp/index.jsp
Request: /testapp/login.do
- user         NEW 42
Request: /testapp/profile.jsp
- user         NOP 42
Request: /testapp/updateprofile.do
- user         CHG 90
Request: /testapp/logout.do
- user         DEL 42
```

__Fontos korlat__: Ez a filter nem ugyanazt meri, mint amit a servlet container-ed. A servlet container-ed minden alkalommal ujra fogja szinkronizalni az adott bean-t, amikor ujra odadobod neki, a filter pedig csak azt tudja nezni hogy a kiserializalt minta valtozott-e. Van olyan eset, amikor nem jelez kapast, pedig a servlet container ujraszinkronizalja a dolgot. Feltetelezzuk hogy nem csinal teljesen hiabavalo munkat az alkalmazasod :)

Es az egeszet ide irtam le: [http://iwillworkforfood.blogspot.com/2008/09/sessionmeter.html](http://iwillworkforfood.blogspot.com/2008/09/sessionmeter.html)
