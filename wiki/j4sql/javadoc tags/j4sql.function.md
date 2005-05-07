---
creationDate        : 2005-04-22 17:34:41 +0200 
author              : kocka 
title               : j4sql/javadoc tags/j4sql.function 
name                : j4sql/javadoc tags/j4sql.function 
layout              : wiki 
path                : j4sql/javadoc tags/j4sql.function 
date                : 2005-05-08 01:00:01 +0200 
version             : 3 
creator             : kocka 
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
```
public class Functions {
  /**
   * Calculates the factorial of the value.
   * 
   * @jsproc.function name="factorial" onNullInput="returns_null" 
   * deterministic="true" sqlAccess="no"
   *
   */
  public static long factorial(int a) {
    long val = 1;
    for(int i=1; i<a; i++){
      l = l*i;
    }
    return l;
  }
}
```
