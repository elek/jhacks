---
creationDate        : 2005-02-04 15:15:26 +0100 
author              : kocka 
title               : Generics 
name                : Generics 
layout              : wiki 
path                : Generics 
date                : 2006-12-07 21:48:53 +0100 
version             : 4 
creator             : kocka 
---
Kis C++-ra emlekezteto szintaktika... Definialhasz akar magad is generic osztalyokat, tipikusan kontenereket (Collections), es megmondhatod hogy milyen tipus lehet benne. Igy nem kell typecastolnod es _elvben_ biztos lehetsz abban hogy az objektum amit kapsz az olyan tipusu mint amire te varsz. A compiler kiabal ha valamiben tevedsz.

Kotelezo tudni: ez csak syntax sugar, belul ugyanaz tortenik mint eddig.

```

List<Customer> customers = new ArrayList<Customer>();

customers.add(new Customer());
//...
for(Customer c : customers) { //itt biztos hogy amit kapunk az oksa
   //...
}

```

Library-k (jar fileok) eseteben okozhat problemat, de osztalyon belul privat kezelve szerintem nagyon qlio.

Mivel a dolog csak syntax sugar, peldaul egy [spring](spring.html) contexten sem kell semmit sem valtoztatni, a spring nem is kell tudja hogy valami megkotes van az adott beanre. Persze ha beletolsz valami mas osztalyt akkor majd lesz exception :)


