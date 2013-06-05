---
creationDate: 1160943573598 
author: karenin 
contentAuthor: karenin 
title: Vararg 
contentUpdateDate: 1160943573598 
name: Vararg 
layout: wiki 
date: 1160943573598 
creator: karenin 
---
Variable Arguments a java 5 egyik új lehetősége. Változó argumentum számú függvényeket lehet vele csinálni. Legtipikusabban a printf-ek használnak ilyet.

Valhogy így néz ki:
{% highlight java %}
public static void main(String... args) \{
        test(new Integer(3),new Long(5));
    \}
    
public static void test(Integer t, Long... args) \{
        System.out.println(args.length);
    \}
{% endhighlight %}

A hárompontos paraméter mindig csak az utolsó lehet, és valójában úgy működik mint egy tömb (ezért is írhattam át a main függvényt).

Ha overload-olunk is, akkor már nagy gazolás lesz belőle.
