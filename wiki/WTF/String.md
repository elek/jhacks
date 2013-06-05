---
creationDate: 1113559634203 
author: kocka 
contentAuthor: kocka 
title: WTF/String 
contentUpdateDate: 1166017089809 
name: WTFString 
layout: wiki 
date: 1166017089809 
creator: kocka 
---
Jaaaaaaaajjjjj! :)

{% highlight java %}
String ize = new String("");
{% endhighlight %}
A -bol: "use of this constructor is unnecessary since Strings are immutable". Vajon mi a francnak tettek bele ezt a konstruktort?

Viszont a [java 1.4](../java%201.4.html) letrehozta a  interface-t, amit a  is implemental, majd a [java 1.5](../java%201.5.html) adott egy  osztalyt, ami szinten, es valtoztathato. Szoval ha valaki nem tudja eldonteni hogy neki most [mutable](../Missing.html) vagy [immutable](../Missing.html) kell, akkor a CharSequence lehet a jo valasz.

Valamint:
{% highlight java %}
"A".equals(ize.substring(0,1)
{% endhighlight %}

Kisbetus vagy nagybetus ures string:)

{% highlight java %}
ize.equalsIgnoreCase("")
{% endhighlight %}

String szam konstans:)
{% highlight java %}
String str = Integer.toString(1);
{% endhighlight %}

Ident :-D
{% highlight java %}
public String indent(int x) \{
 return "........................................................................................................................"
 .substring(0,x);
\}
{% endhighlight %}


Hogyan konvertáljunk valamit String-é :)
{% highlight java %}
String string = (Object)map.get("something")+"";
{% endhighlight %}
