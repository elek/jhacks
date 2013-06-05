---
creationDate: 1113999653818 
author: kocka 
contentAuthor: kocka 
title: java 1.5/For ciklus 
contentUpdateDate: 1180547291300 
name: java 1.5For ciklus 
layout: wiki 
date: 1180547291300 
creator: kocka 
---
A [java 1.5](../java%201.5.html) uj ciklusszervezese.

Nehany betut meg akartak takaritani nekunk, es ez sikerult is.

{% highlight java %}

String[] array = new String[] \{"Ize","Hogyishivjak","Tood","Biszbasz"\};
for(String s: array)\{
  System.out.println(s);
\}

{% endhighlight %}

Csodas kombinacioban lehet hasznalni a [generics](../Generics.html)-szel:

{% highlight java %}

Collection<String> col;
...
for(String s:col)\{
  System.out.println(s);
\}

{% endhighlight %}

A l?nyeg annyi, hogy amit iter?l az ember, az Iterable kell hogy legyen.

Hat igen, sajna az iterator vagy az index ertek ilyenkor nem elerheto, ilyesmit akkor erdemes csinalni ha megvagyunk nelkule. Kb az esetek 60-70 szazalekaban. A dolog m?gink?b ?rdekes lesz a [java 1.7](../java%201.7.html) [closure](../Missing.html) szintaxis?val, err?l egyel?re csak ?tletek vannak.

Roviden ennyi, azert nagyon ql. Az [eclipse](../Eclipse.html) es a [netbeans](../Netbeans.html) is tamogassa.

__Cikkek__:

*   [Nuances of the Java 5.0 for-each Loop](http://today.java.net/pub/a/today/2006/11/07/nuances-of-java-5-for-each-loop.html)
