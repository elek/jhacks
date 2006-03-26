---
creationDate        : 2005-04-20 14:20:53 +0200 
author              : admin 
title               : java 1.5/For ciklus 
name                : java 1.5/For ciklus 
layout              : wiki 
path                : java 1.5/For ciklus 
date                : 2006-03-26 01:48:11 +0100 
version             : 1 
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

Hat roviden ennyi, azert nagyon ql. Az [eclipse](../Eclipse.html) es a [netbeans](../Netbeans.html) is tamogassa.
