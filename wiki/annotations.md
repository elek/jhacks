---
creationDate        : 2005-02-03 08:58:49 +0100 
author              : admin 
title               : annotations 
name                : annotations 
layout              : wiki 
path                : annotations 
date                : 2006-03-26 01:43:05 +0100 
version             : 1 
creator             : kocka 
---
Az annotations uj feature a [java 1.5](java%201.5.html)ben, amivel metainformaciot adhatsz hozza az osztalyokhoz, metodusokhoz, tagvaltozoidhoz, es ezeket egyszeru [reflection](reflection.html) segitsegevel ki is olvashatod.

pelda:
```
@MetaData4Class(
  meta = 1,
  data = "meta"
)
public class Demo {
  @MetaData4Method( bla = "bla")
  public void method() {}
}

```

Ez kicsit odaut az olyan regi de jol bevallt cuccosoknak mint az [xdoclet](XDoclet.html) peldaul, de azert ne temessuk meg :)

Specifikacio: [JSR 175](http://www.jcp.org/en/jsr/detail?id=175)

cikkek:

*   [ Annotations to the rescue](http://www.javaworld.com/javaworld/jw-08-2005/jw-0801-annotations_p.html)
