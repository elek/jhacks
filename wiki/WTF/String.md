---
creationDate        : 2005-04-15 12:07:14 +0200 
author              : admin 
title               : WTF/String 
name                : WTF/String 
layout              : wiki 
path                : WTF/String 
date                : 2006-03-26 01:43:02 +0100 
version             : 1 
creator             : kocka 
---
Jaaaaaaaajjjjj! :)

```
String ize = new String("");
```
A [java.lang.String](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html)-bol: "use of this constructor is unnecessary since Strings are immutable". Vajon mi a francnak tettek bele ezt a konstruktort?

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
