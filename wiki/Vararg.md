---
creationDate        : 2006-10-15 22:19:33 +0200 
author              : karenin 
title               : Vararg 
name                : Vararg 
layout              : wiki 
path                : Vararg 
date                : 2006-10-15 22:19:33 +0200 
version             : 1 
creator             : karenin 
---
Variable Arguments a java 5 egyik új lehetősége. Változó argumentum számú függvényeket lehet vele csinálni. Legtipikusabban a printf-ek használnak ilyet.

Valhogy így néz ki:
```
public static void main(String... args) {
        test(new Integer(3),new Long(5));
    }
    
public static void test(Integer t, Long... args) {
        System.out.println(args.length);
    }
```

A hárompontos paraméter mindig csak az utolsó lehet, és valójában úgy működik mint egy tömb (ezért is írhattam át a main függvényt).

Ha overload-olunk is, akkor már nagy gazolás lesz belőle.
