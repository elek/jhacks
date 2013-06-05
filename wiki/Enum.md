---
creationDate: 1160943816963 
author: karenin 
contentAuthor: karenin 
title: Enum 
contentUpdateDate: 1160943832903 
name: Enum 
layout: wiki 
date: 1160943832903 
creator: karenin 
---
[Java 1.5](java%201.5.html) újítás, típusos felsorolás konstanst lehet vele ízlésesen csinálni.

Definíciója az osztályéhoz hasonló:

{% highlight java %}
public enum Evszak \{
    TAVASZ, NYAR, OSZ, TEL
\}
{% endhighlight %}

Jó, mert:

*   típusos, azaz lehet Evszak típusú változó, ami csak az adott értékeket veheti fel
*   lehet rá iterátort kapni, és végignézni az értékeit
*   switch-ben használható
*   a háttérben int-ek mennek, ezért gyors
