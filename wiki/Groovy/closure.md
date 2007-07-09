---
creationDate        : 2006-10-18 12:33:38 +0200 
author              : kocka 
title               : Groovy/closure 
name                : Groovy/closure 
layout              : wiki 
path                : Groovy/closure 
date                : 2007-07-09 22:05:52 +0200 
version             : 8 
creator             : kocka 
---
A closure a [groovy](../Groovy.html)ban kb olyan mint egy callback osztaly [java](../java.html)ban, csak annal kicsit rovidebben meg lehet fogalmazni :)

peldaul van egy listank aminek minden elemere kiiratnank +1-et a kimenetre.
```

def plusoneclos = { println it + 1}

[1,2,3,4].each(plusoneclos)

```

nagyon kompakt, meg elsore nagyon erthetetlen, de azta jo moka.

Lasd meg: [groovy/closure](../Groovy/closure.html)
