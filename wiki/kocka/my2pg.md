---
creationDate: 1201211369915 
author: kocka 
contentAuthor: kocka 
title: My2pg 
contentUpdateDate: 1202767612259 
name: kockamy2pg 
layout: wiki 
date: 1202767612259 
creator: kocka 
---
Kis [python](python.html) [script](scripting.html) [mysql](MySQL.html) dumpok [PostgreSQL-re](PostgreSQL.html) konvertálására.


Használd így:

{% highlight java %}
gzip -dcf enwiki-20080103-categorylinks.sql.gz | python my2pg.py -c | psql wikipedia
{% endhighlight %}

Van persze [perl](perl.html) verzió is, de nekem nem működött, 2002 óta senki nem nyúlt hozzá :-( Perl-ül meg már nem akarok érteni :)

Ennyi, írjátok át ami nem tetszik!

Kozka.
