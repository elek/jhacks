---
creationDate: 1114184081620 
author: kocka 
contentAuthor: kocka 
title: j4sql/javadoc tags/j4sql.function 
contentUpdateDate: 1115506801828 
name: j4sqljavadoc tagsj4sql.function 
layout: wiki 
date: 1115506801828 
creator: kocka 
---
A jsproc.function taggel egyszeruen keszithetunk SQL funkciokat.

Attributumai:

Attributum|kotelezo|leiras|default
name|igen|az UDF neve
properties|nem|[RDBMS](../../RDBMS.html) specifikus UDF tulajdonsagok
security|nem|melyik felhasznalokent hivodjon meg a kod? 'invoker' vagy 'definer'|'invoker'
deterministic|nem|A funkcio ugyanarra az inputra ugyanazt az outputot adja-e?|false
sqlAccess|nem|A funkcio adatbazis hozzaferese. 'no', 'contains', 'reads', 'modifies'| 'contains'
onNullInput|nem|NULL parameterek eseten meg kell-e hivni? 'called' vagy 'returns_null'|'calles'


Pelda:
{% highlight java %}
public class Functions \{
  /**
   * Calculates the factorial of the value.
   * 
   * @jsproc.function name="factorial" onNullInput="returns_null" 
   * deterministic="true" sqlAccess="no"
   *
   */
  public static long factorial(int a) \{
    long val = 1;
    for(int i=1; i<a; i++)\{
      l = l*i;
    \}
    return l;
  \}
\}
{% endhighlight %}
