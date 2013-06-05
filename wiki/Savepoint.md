---
creationDate: 1105447601097 
author: kocka 
contentAuthor: kocka 
title: Savepoint 
contentUpdateDate: 1105447601097 
name: Savepoint 
layout: wiki 
date: 1105447601097 
creator: kocka 
---
A Savepoint vajon mi.

Az [sql](SQL.html) szabvany eloirja az [RDBMS](RDBMS.html)-ek szamara egy olyan lehetoseg biztositasat, amivel a tranzakcio egy resze visszagorgetheto. Egeszen ponstosana  legutobbi muveletek.

{% highlight java %}

begin transaction;

create table a (v varchar);

create savepoint hello0;

insert into a values ('hello1')

create savepoint hello1;

insert into a values ('hello2')

create savepoint hello2;

rollback to hello1;
{% endhighlight %}

Ezek utan a tablaban csak a 'hello1' kell hogy legyen. Az erdekes a dologban az, hogy beagyazott tranzakciokkal is el lehet erni ugyanezt, szvsz az kicsit jobban passzol mindenhez...
