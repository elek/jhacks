---
creationDate        : 2006-10-18 12:33:38 +0200 
author              : kocka 
title               : Groovy/closure 
name                : Groovy/closure 
layout              : wiki 
path                : Groovy/closure 
date                : 2007-10-25 17:36:46 +0200 
version             : 9 
creator             : kocka 
---
A closure a [groovy](../Groovy.html)ban kb olyan mint egy callback osztaly [java](../java.html)ban (bár már nagyban forr a vita a [java 1.7](../java%201.7.html) [closures](../closures.html) körül), csak annal kicsit rovidebben meg lehet fogalmazni :)

peldaul van egy listank aminek minden elemere kiiratnank +1-et a kimenetre.
```

def plusoneclos = { println it + 1}

[1,2,3,4].each(plusoneclos)

```

nagyon kompakt, meg elsore nagyon erthetetlen, de azta jo moka.

Lasd meg: [closures](../closures.html)
