---
creationDate: 1113819532508 
author: kocka 
contentAuthor: kocka 
title: WTF/Exception 
contentUpdateDate: 1113824136228 
name: WTFException 
layout: wiki 
date: 1113824136228 
creator: kocka 
---
Megoldas az exception okanak titokban tartasara.

{% highlight java %}

    try \{
      ize = hello();
    \} catch (Exception ex) \{
      if (ex.getMessage() != null)
        throw new RuntimeException(e.getMessage());
      throw new RuntimeException();
    \}
{% endhighlight %}

Az hogy mi lehetett az oka az ilyen nehezen emesztheto hibakezelesnek, [itt](http://c2.com/cgi/wiki?ThrowsExceptionByDefault) irja le egy cikk, utanna azt is leirjak hogy miert hibas.
