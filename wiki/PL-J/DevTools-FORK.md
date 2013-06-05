---
creationDate: 1113297150750 
author: kocka 
contentAuthor: kocka 
title: PL-J/DevTools-FORK 
contentUpdateDate: 1113299464957 
name: PL-JDevTools-FORK 
layout: wiki 
date: 1113299464957 
creator: kocka 
---
This is the ongoing spec-kinda-thing of the project intended to fork out from [PL-J](../PL-J.html) [PL-J/DevTools](../PL-J/DevTools.html). It contains nothing more than we have already agreed in.

See also: [PL-J/DevTools-FORK/dblayer](../PL-J/DevTools-FORK/dblayer.html)

{% highlight java %}
public class JSProc1 \{

/**
 * A very stupid UDF.
 * 
 * @jsproc.function name="int_add"
 */
public static int add(int arg1, int arg2) \{
 return arg1 + arg2;
\}

\}
{% endhighlight %}

An example of the generated code:
{% highlight java %}

create function int_add(integer, integer) returns integer as
'
class=JSProc1
method=add
' language 'PL-J';

comment on function int_add(integer, integer) is 'A very stupid UDF.';

{% endhighlight %}
