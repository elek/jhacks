---
creationDate: 1107527466554 
author: kocka 
contentAuthor: kocka 
title: Autoboxing 
contentUpdateDate: 1142091500887 
name: Autoboxing 
layout: wiki 
date: 1142091500887 
creator: kocka 
---
Autoboxing/unboxing

Egy mokas kis mechanizmus a [java 1.5](java%201.5.html)-ben arra hogy az elemi tipusok kompatibilisek legyenek az osztaly megfelelojukkel. 

Syntax sugar, azaz valojaban objektum letrehozassal es metodushivassal mukodik.<br/>
Szemleltetesul:

Alapbol igy megy:<br/>
{% highlight java %}
Integer i = 1;
int j = i;
{% endhighlight %}

Nyilvan ha elemi valtozonak null-t akarsz adni ertekul valahogy akkor [NPE](NPE.html) keletkezik:<br/>
{% highlight java %}
Integer i = null;
int j = i;
{% endhighlight %}
Ennek azert nyilvan vannak kevesbe evidens esetei is, peldaul amikor fuggvenyhivas ad vissza Long-kent nullt, amibol egybol long-ot csinlasz. Amikor pedig method signature-ben valtoztatod a parametert objektumbol elemi tipusba vagy vissza, akkor jobb egy full clean rebuild.

Cikkek:

*   http://today.java.net/pub/a/today/2005/03/24/autoboxing.html - ez a cikk bovebben leirja milyen aknakra lehet lepni az autoboxing mezon.
