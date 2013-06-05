---
creationDate: 1112609139009 
author: renszarv 
contentAuthor: renszarv 
title: WTF/DatePool 
contentUpdateDate: 1112611336536 
name: WTFDatePool 
layout: wiki 
date: 1112611336536 
creator: renszarv 
---
Már nem production kód, de az volt (emlékezetből, csak a lényeg)

{% highlight java %}

 private static int datePos = 0;
private static Date[] datePool = new Date[16];


 public static String toString(long time) \{
     Date date = datePool[datePos++ % datePool.length];
     date.setTime(time);
     return date.toString();
 \}
{% endhighlight %}

 Persze bármilyen szinkronizáció nélkül ... 
