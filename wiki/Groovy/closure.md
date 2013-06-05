---
creationDate: 1161167618512 
author: kocka 
contentAuthor: kocka 
title: Groovy/closure 
contentUpdateDate: 1193326626882 
name: Groovyclosure 
layout: wiki 
date: 1193326626882 
creator: kocka 
---
A closure a [groovy](../Groovy.html)ban kb olyan mint egy callback osztaly [java](../java.html)ban (bár már nagyban forr a vita a [java 1.7](../java%201.7.html) [closures](../closures.html) körül), csak annal kicsit rovidebben meg lehet fogalmazni :)

peldaul van egy listank aminek minden elemere kiiratnank +1-et a kimenetre.
{% highlight java %}

def plusoneclos = \{ println it + 1\}

[1,2,3,4].each(plusoneclos)

{% endhighlight %}

nagyon kompakt, meg elsore nagyon erthetetlen, de azta jo moka.

Lasd meg: [closures](../closures.html)


