---
creationDate        : 2008-01-24 22:49:29 +0100 
author              : kocka 
title               : My2pg 
name                : kocka/my2pg 
layout              : wiki 
path                : kocka/my2pg 
date                : 2008-02-11 23:06:52 +0100 
version             : 7 
creator             : kocka 
---
Kis [python](../python.html) [script](../scripting.html) [mysql](../MySQL.html) dumpok [PostgreSQL-re](../PostgreSQL.html) konvertálására.


Használd így:

```
gzip -dcf enwiki-20080103-categorylinks.sql.gz | python my2pg.py -c | psql wikipedia
```

Van persze [perl](../perl.html) verzió is, de nekem nem működött, 2002 óta senki nem nyúlt hozzá :-( Perl-ül meg már nem akarok érteni :)

Ennyi, írjátok át ami nem tetszik!

Kozka.
