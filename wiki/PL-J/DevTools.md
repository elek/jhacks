---
creationDate        : 2004-12-22 10:18:39 +0100 
author              : admin 
title               : PL-J/DevTools 
name                : PL-J/DevTools 
layout              : wiki 
path                : PL-J/DevTools 
date                : 2006-03-26 01:42:49 +0100 
version             : 1 
creator             : kocka 
---
__FORKOLVA__

Ez a package kikerult a [PL-J](../PL-J.html) alol es alapos refactoring utan [J4SQL](../j4sql.html) lett az uj othona.

A [PL-J](../PL-J.html) DevTools egy kulon projectben keszulo kis taszkok ([ant](../ant.html)hoz es [maven](../maven.html)hez) keszlete lesz java tarolt eljarasok keszitesehez. Eddig igazabol a tervezes zajlik. Egy nagyon buta peldaval hogy mit fog csinalni:

[CVS](../CVS.html): A DevTools elerheto a [PL-J](../PL-J.html) [CVS](../CVS.html)ben.<br/>
web cvs: [http://cvs.plj.codehaus.org/pl-j-devtools/](http://cvs.plj.codehaus.org/pl-j-devtools/)



Jelenleg meg eleg minimalis funckionalitasa van, csak [PostgreSQL](../PostgreSQL.html)-[PL-J](../PL-J.html) kombinacora.

```
public class JSProc1 {

/**
 * A very stupid UDF.
 * 
 * @jsproc.udf name="int_add"
 * @jsproc.return integer
 * @jsproc.param arg1 in integer
 * @jsproc.param arg2 in integer
 * @jsproc.properties immutable
 */
public static int add(int arg1, int arg2) {
 return arg1 + arg2;
}

}
```

Es ebbol neked legeneralja majd a kovetkezo SQL kodot [PostgreSQL](../PostgreSQL.html)-hez es [Pl-J](../PL-J.html)-hez:

```

create function int_add(integer, integer) returns integer as
'
class=JSProc1
method=add
' language 'PL-J' immutable

comment on function int_add(integer, integer) is 'A very stupid UDF.';

```

Hat KB ennyi. Na most az extra az annyi, hogy nem csak [PostgreSQL](../PostgreSQL.html)/[PL-J](../PL-J.html)-re generalna kodot, hanem mas DB-kre is, [Db2](../DB2.html), [Oracle](../Oracle.html), satobbi...

Na ezzel kapcsolatban [PLjava](../pljava.html) Thomas beszolt nemreg, hogy o irt [annotations](../annotations.html)t amit szerinte hasznalnom kellene. Meg az sem biztos hogy egyaltalan implementalni fogom az o annotacioit, ugyanis:

*   A [PL-J](../PL-J.html) tipus mappelo rendszere N:N mappeles, mig a [PLJava](../pljava.html) 1:1, a fenti [annotations](../annotations.html) pont erre epul ra, de nagyon
*   Na es mi legyen a java 1.4 juzerekkel?
*   Na es mizujs a szabvanyokkal es a portolhatosaggal?
