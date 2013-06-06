---
creationDate        : 2008-04-15 15:02:37 +0200 
author              : kocka 
title               : kocka/jndi-postprocessor 
name                : kocka/jndi-postprocessor 
layout              : wiki 
path                : kocka/jndi-postprocessor 
date                : 2008-04-15 19:51:13 +0200 
version             : 5 
creator             : kocka 
---
Egy [JNDI](../JNDI.html) postprocessor [springhez](../spring.html). A spring alkalmazás kontextus startolása után végigtúrja a bean definicióidat és megprobálja vagy a teljes bean-eket vagy a tulajdonságaikat lehelyettesíteni a JNDI fa megfelelő objektumával.

Egyszerű és buta :)

```
<bean id="overloader" class="net.anzix.jhacks.jndi.JNDIPostProcessor">
  <constructor-arg><value>java:comp/env/test</value></constructor-arg>
</bean>
```
Ez a fenti snippet a test alól fogja próbálni behelyettesítgetni a [beanjeiet](../pojo.html) JNDI resourceokkal.

Linkek:

*   [Alapötlet](http://iwillworkforfood.blogspot.com/2008/04/tls-konfigurci-hovatevsrl.html)
