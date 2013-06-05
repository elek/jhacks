---
creationDate: 1108377443130 
author: kocka 
contentAuthor: kocka 
title: XPath 
contentUpdateDate: 1112962591957 
name: XPath 
layout: wiki 
date: 1112962591957 
creator: kocka 
---
(Ettol a szotol a munkehelyemen egyesek rohogni kezdenek, masok sirnak. En hol ez hol az...)

Egy [w3c](w3c.html) szabvany megoldas a [XML](XML.html) dokumentum bizonyos reszenek meghatarozasara.

nagyon ecceru pelda:
{% highlight java %}
<person name="Kovacs Bela">
  <age>25</age>
</person>
{% endhighlight %}

igy erjuk el az &lt;age&gt; adatot: //person/age

Lasd: 

*   implementaciok: [jaxen](jaxen.html)
*   kapcsolodo technologiak: [xquery](XQuery.html), [xml](XML.html)
