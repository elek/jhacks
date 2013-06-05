---
creationDate: 1225653755672 
author: zmb 
contentAuthor: zmb 
title: WTF/Veszelyes konstans 
contentUpdateDate: 1225653755672 
name: WTFVeszelyes konstans 
layout: wiki 
date: 1225653755672 
creator: zmb 
---
Sokszor elofordul, hogy bizonyos ertekeket konstansokba rakunk, es azokra hivatkozunk. A kovetkezo kis kodreszletben valamiert a fejleszo ugy gondolta, hogy enum segitsegevel jobban megoldhato a problema, mint egyszeru konstanssal.

{% highlight java %}
protected int pageLength = PAGE_LENGTH.LENGTH_10.getPageLength();

public static enum PAGE_LENGTH \{
	LENGTH_10 \{
		public int getPageLength() \{
			return 10;
		\}

	\},
	LENGTH_25 \{
		public int getPageLength() \{
			return 25;
		\}
	\},
	LENGTH_50 \{
		public int getPageLength() \{
			return 50;
		\}
	\};

	public abstract int getPageLength();
\}
{% endhighlight %}
