---
creationDate: 1128345443490 
author: suhaig 
contentAuthor: suhaig 
title: WTF/Unsupported constructor 
contentUpdateDate: 1128345443490 
name: WTFUnsupported constructor 
layout: wiki 
date: 1128345443490 
creator: suhaig 
---
Valaki esetleg megmagyarazhatna, koszonom.
<br/>
{% highlight java %}
private ValamiClass() throws java.lang.UnsupportedOperationException \{
    throw new java.lang.UnsupportedOperationException("Illegal constructor call");
\}
{% endhighlight %}
