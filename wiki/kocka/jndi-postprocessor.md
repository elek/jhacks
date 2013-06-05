---
creationDate: 1208264557904 
author: kocka 
contentAuthor: kocka 
title: kocka/jndi-postprocessor 
contentUpdateDate: 1208281873453 
name: kockajndi-postprocessor 
layout: wiki 
date: 1208281873453 
creator: kocka 
---
Egy [JNDI](../JNDI.html) postprocessor [springhez](../spring.html). A spring alkalmazás kontextus startolása után végigtúrja a bean definicióidat és megprobálja vagy a teljes bean-eket vagy a tulajdonságaikat lehelyettesíteni a JNDI fa megfelelő objektumával.

Egyszerű és buta :)

{% highlight java %}
<bean id="overloader" class="net.anzix.jhacks.jndi.JNDIPostProcessor">
  <constructor-arg><value>java:comp/env/test</value></constructor-arg>
</bean>
{% endhighlight %}
Ez a fenti snippet a test alól fogja próbálni behelyettesítgetni a [beanjeiet](../pojo.html) JNDI resourceokkal.

Linkek:

*   [Alapötlet](http://iwillworkforfood.blogspot.com/2008/04/tls-konfigurci-hovatevsrl.html)
