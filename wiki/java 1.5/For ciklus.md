---
creationDate        : 2005-04-20 14:20:53 +0200 
author              : kocka 
title               : java 1.5/For ciklus 
name                : java 1.5/For ciklus 
layout              : wiki 
path                : java 1.5/For ciklus 
date                : 2007-05-30 19:48:11 +0200 
version             : 4 
creator             : kocka 
---
A [java 1.5](../java%201.5.html) uj ciklusszervezese.

Nehany betut meg akartak takaritani nekunk, es ez sikerult is.

```

String[] array = new String[] {"Ize","Hogyishivjak","Tood","Biszbasz"};
for(String s: array){
  System.out.println(s);
}

```

Csodas kombinacioban lehet hasznalni a [generics](../Generics.html)-szel:

```

Collection<String> col;
...
for(String s:col){
  System.out.println(s);
}

```

A l?nyeg annyi, hogy amit iter?l az ember, az Iterable kell hogy legyen.

Hat igen, sajna az iterator vagy az index ertek ilyenkor nem elerheto, ilyesmit akkor erdemes csinalni ha megvagyunk nelkule. Kb az esetek 60-70 szazalekaban. A dolog m?gink?b ?rdekes lesz a [java 1.7](../java%201.7.html) [closure](../Missing.html) szintaxis?val, err?l egyel?re csak ?tletek vannak.

Roviden ennyi, azert nagyon ql. Az [eclipse](../Eclipse.html) es a [netbeans](../Netbeans.html) is tamogassa.

__Cikkek__:

*   [Nuances of the Java 5.0 for-each Loop](http://today.java.net/pub/a/today/2006/11/07/nuances-of-java-5-for-each-loop.html)
