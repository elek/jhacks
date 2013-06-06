---
creationDate        : 2005-02-03 08:58:49 +0100 
author              : kocka 
title               : annotations 
name                : annotations 
layout              : wiki 
path                : annotations 
date                : 2008-03-23 09:47:38 +0100 
version             : 11 
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
*   [junit](junit.html) 4.x-es széria
*   [testNG](testng.html) kezdetektől fogva
*   [jsr-181](jsr-181.html) [webservices](WebServices.html) annotations
*   [guice](guice.html) [ioc](ioc.html) framework.
*   [JPA](JPA.html), [hibernate](Hibernate.html)
*   Az új [J2EE](j2ee.html) standardban is például [servleteket](servlet_jsp.html) így (is) lehet majd a [webalkalmazásba](webapp.html) beledobni.
*   vagy bármi, amihez metaadatokat akarhatsz írni a kódba. _(Azért itt ezt valahogy ésszerű keretek közt érdemes tartani, nem akármiért költözött ki a kódból a konfiguráció :) )_

cikkek:

*   [ Annotations to the rescue](http://www.javaworld.com/javaworld/jw-08-2005/jw-0801-annotations_p.html)


