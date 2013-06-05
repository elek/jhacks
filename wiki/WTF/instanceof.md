---
creationDate: 1129901689912 
author: kocka 
contentAuthor: kocka 
title: WTF/instanceof 
contentUpdateDate: 1129908797162 
name: WTFinstanceof 
layout: wiki 
date: 1129908797162 
creator: kocka 
---
Emberek, az instanceof operator @deprecated. Most indiai kollegaink bemutatnak egy teljesen uj es hatekony megoldast a lehelyettesitesere:

{% highlight java %}
if(obj.toString().startsWith("biszbasz")) \{
 ...
\}
{% endhighlight %}

Na? Remelem fajt :-D
