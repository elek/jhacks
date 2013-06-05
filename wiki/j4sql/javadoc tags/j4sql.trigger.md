---
creationDate: 1114184044443 
author: kocka 
contentAuthor: kocka 
title: j4sql/javadoc tags/j4sql.trigger 
contentUpdateDate: 1115406232135 
name: j4sqljavadoc tagsj4sql.trigger 
layout: wiki 
date: 1115406232135 
creator: kocka 
---
A triggerket ketfelekeppen lehet deklaralni:
a. gyors es megszokott megoldas: nem definialunk neki kulon funkciot, hanem a definialt funkcio csak a triggerhez szolgal
a. definialunk egy funkciot, es arra akarhany triggert is tehetunk.

Pelda1:
{% highlight java %}

...
/**
 * Egy eleg extrem eset, tobb trigger ugyanarra a metodusra.
 * 
 * @j4sql.function name="ize_trig_fn"
 * @j4sql.trigger name="ize_trig1" 
 * @j4sql.trigger name="ize_trig2" 
 * 
 */
public static void doInsertEvent()\{

\}

{% endhighlight %}
