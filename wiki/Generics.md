---
creationDate: 1107526526756 
author: kocka 
contentAuthor: kocka 
title: Generics 
contentUpdateDate: 1165524533292 
name: Generics 
layout: wiki 
date: 1165524533292 
creator: kocka 
---
Kis C++-ra emlekezteto szintaktika... Definialhasz akar magad is generic osztalyokat, tipikusan kontenereket (Collections), es megmondhatod hogy milyen tipus lehet benne. Igy nem kell typecastolnod es _elvben_ biztos lehetsz abban hogy az objektum amit kapsz az olyan tipusu mint amire te varsz. A compiler kiabal ha valamiben tevedsz.

Kotelezo tudni: ez csak syntax sugar, belul ugyanaz tortenik mint eddig.

{% highlight java %}

List<Customer> customers = new ArrayList<Customer>();

customers.add(new Customer());
//...
for(Customer c : customers) \{ //itt biztos hogy amit kapunk az oksa
   //...
\}

{% endhighlight %}

Library-k (jar fileok) eseteben okozhat problemat, de osztalyon belul privat kezelve szerintem nagyon qlio.

Mivel a dolog csak syntax sugar, peldaul egy [spring](spring.html) contexten sem kell semmit sem valtoztatni, a spring nem is kell tudja hogy valami megkotes van az adott beanre. Persze ha beletolsz valami mas osztalyt akkor majd lesz exception :)


