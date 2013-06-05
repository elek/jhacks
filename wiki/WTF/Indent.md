---
creationDate: 1112530311379 
author: kocka 
contentAuthor: kocka 
title: WTF/Indent 
contentUpdateDate: 1112530485073 
name: WTFIndent 
layout: wiki 
date: 1112530485073 
creator: kocka 
---
Indantalas java-ban :)

Nem az a tipikus atomszar, de jot rohogtem rajta. Ez nem vicc, ez eles :) Pont ezert veszelyes.

{% highlight java %}
    /**
     * Returns indent string.
     */
    public static String indent(int i) \{
	return  ("..........................."
               +"..........................."
               +"..........................."
               +"..........................."
               +"..........................."
               +"..........................."
               +"..........................."
               +"..........................."
               +"..........................."
               +"..........................."
               +"...........................")
		   .substring(0, i * 1);
    \}
{% endhighlight %}
