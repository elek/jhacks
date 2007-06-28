---
creationDate        : 2006-10-18 12:33:38 +0200 
author              : kocka 
title               : Groovy/closure 
name                : Groovy/closure 
layout              : wiki 
path                : Groovy/closure 
date                : 2007-06-28 09:47:57 +0200 
version             : 6 
creator             : kocka 
---
A closure a [groovy](../Groovy.html)ban kb olyan mint egy callback osztaly [java](../java.html)ban, csak annal kicsit rovidebben meg lehet fogalmazni :)

peldaul van egy listank aminek minden elemere kiiratnank +1-et a kimenetre.
```

def plusoneclos = { println it + 1}

[1,2,3,4].each(plusoneclos)

```

nagyon kompakt, meg elsore nagyon erthetetlen, de azta jo moka.

Linkek: 

*   [Closures for java - javapolis 2006](http://www.bejug.org/confluenceBeJUG/display/PARLEYS/Closures+for+Java)
*   [Closures for java](http://www.oreillynet.com/onjava/blog/2006/08/will_we_have_closures_in_java.html) ([java 1.7](../java%201.7.html), es csak proposal)
*   [Closures in Java 7.0](http://www.oreillynet.com/onjava/blog/2006/12/closures_in_java_70.html)


