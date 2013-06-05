---
creationDate: 1165413116595 
author: kocka 
contentAuthor: kocka 
title: assertion 
contentUpdateDate: 1165413116595 
name: assertion 
layout: wiki 
date: 1165413116595 
creator: kocka 
---
Az assertion a [java 1.4](java%201.4.html) erdekessege volt, az alapgondolat az, hogy ha a VM-et assertion modban futtatod (-ea parameterrel), akkor az assert pontoknal ha a feltetel nem teljesul akkor ott  kepzodik. Ami valoszinuleg kinyirja a [thread](thread.html)edet mert tokre nem illik elkapni.

Kb ennyi a hasznalata:
{% highlight java %}
assert 0 < value;
{% endhighlight %}

Ez nem sok embernek koltozott a szivebe, mert en egyetlen egyszer nem lattam senkit aki hasznalna. Inkab [unit testing](unit%20testing.html). Mindenesetre [test](test.html) futtatashoz erdekes lehetoseg, a semminel meg mindig jobb.


