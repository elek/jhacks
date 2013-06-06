---
creationDate        : 2005-04-15 12:07:14 +0200 
author              : kocka 
title               : WTF/String 
name                : WTF/String 
layout              : wiki 
path                : WTF/String 
date                : 2006-12-13 14:38:09 +0100 
version             : 8 
creator             : kocka 
---
Jaaaaaaaajjjjj! :)

```
String ize = new String("");
```
A [java.lang.String](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html)-bol: "use of this constructor is unnecessary since Strings are immutable". Vajon mi a francnak tettek bele ezt a konstruktort?

Viszont a [java 1.4](../java%201.4.html) letrehozta a [java.lang.CharSequence](http://docs.oracle.com/javase/7/docs/api/java/lang/CharSequence.html) interface-t, amit a [java.lang.String](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html) is implemental, majd a [java 1.5](../java%201.5.html) adott egy [java.lang.StringBuilder](http://docs.oracle.com/javase/7/docs/api/java/lang/StringBuilder.html) osztalyt, ami szinten, es valtoztathato. Szoval ha valaki nem tudja eldonteni hogy neki most [mutable](../Missing.html) vagy [immutable](../Missing.html) kell, akkor a CharSequence lehet a jo valasz.

Valamint:
```
"A".equals(ize.substring(0,1)
```

Kisbetus vagy nagybetus ures string:)

```
ize.equalsIgnoreCase("")
```

String szam konstans:)
```
String str = Integer.toString(1);
```

Ident :-D
```
public String indent(int x) {
 return "........................................................................................................................"
 .substring(0,x);
}
```


Hogyan konvertáljunk valamit String-é :)
```
String string = (Object)map.get("something")+"";
```
