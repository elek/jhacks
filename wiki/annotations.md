---
creationDate        : 2005-02-03 08:58:49 +0100 
author              : kocka 
title               : annotations 
name                : annotations 
layout              : wiki 
path                : annotations 
date                : 2007-05-29 16:24:48 +0200 
version             : 7 
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

A dolog egy érdekessége hogy mekkora hatással lett a frameworkökre a technológia, kifejezetten annotations alapú rendszerek láttak napvilágot az 2006 első felétől egyre inkáb:

*   [Tapestry](tapestry.html) 4.x-től, de az 5.x már nagyon
*   [struts/struts 2](struts/struts%202.html)

cikkek:

*   [ Annotations to the rescue](http://www.javaworld.com/javaworld/jw-08-2005/jw-0801-annotations_p.html)


