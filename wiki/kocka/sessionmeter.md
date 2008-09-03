---
creationDate        : 2008-09-03 00:42:17 +0200 
author              : kocka 
title               : Sessionmeter 
name                : kocka/sessionmeter 
layout              : wiki 
path                : kocka/sessionmeter 
date                : 2008-09-03 08:25:17 +0200 
version             : 3 
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
Request: /testapp/updateprofile.so
- user         CHG 90
Request: /testapp/logout.do
- user         DEL 42
```
