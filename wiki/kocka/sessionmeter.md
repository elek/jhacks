---
creationDate        : 2008-09-03 00:42:17 +0200 
author              : kocka 
title               : Sessionmeter 
name                : kocka/sessionmeter 
layout              : wiki 
path                : kocka/sessionmeter 
date                : 2008-09-03 22:36:16 +0200 
version             : 7 
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

Es az egeszet ide irtam le: [http://iwillworkforfood.blogspot.com/2008/09/sessionmeter.html](http://iwillworkforfood.blogspot.com/2008/09/sessionmeter.html)
