---
creationDate: 1122977764855 
author: suhaig 
contentAuthor: suhaig 
title: WTF/BEGIN TRANSACTION 
contentUpdateDate: 1122977764855 
name: WTFBEGIN TRANSACTION 
layout: wiki 
date: 1122977764855 
creator: suhaig 
---
Szükséges ehhez bármiféle megjegyzés?

{% highlight java %}
public int beginTransaction() throws SpecificException
\{
	try
	\{
		if (DB_TYPE.equals(DBTYPE_SQLSERVER))
			executeUpdate("BEGIN TRANSACTION", null);
		else
			return 0;
	\}
	catch (Exception ex)
	\{
		throw new SpecificException(SpecificException.ERROR_IN_DBCONNECTION);
	
	\}
\}
{% endhighlight %}
