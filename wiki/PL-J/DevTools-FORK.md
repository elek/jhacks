---
creationDate        : 2005-04-12 11:12:30 +0200 
author              : admin 
title               : PL-J/DevTools-FORK 
name                : PL-J/DevTools-FORK 
layout              : wiki 
path                : PL-J/DevTools-FORK 
date                : 2006-03-26 01:42:49 +0100 
version             : 1 
creator             : kocka 
---
This is the ongoing spec-kinda-thing of the project intended to fork out from [PL-J](../PL-J.html) [PL-J/DevTools](../PL-J/DevTools.html). It contains nothing more than we have already agreed in.

See also: [PL-J/DevTools-FORK/dblayer](../PL-J/DevTools-FORK/dblayer.html)

```
public class JSProc1 {

/**
 * A very stupid UDF.
 * 
 * @jsproc.function name="int_add"
 */
public static int add(int arg1, int arg2) {
 return arg1 + arg2;
}

}
```

An example of the generated code:
```

create function int_add(integer, integer) returns integer as
'
class=JSProc1
method=add
' language 'PL-J';

comment on function int_add(integer, integer) is 'A very stupid UDF.';

```
