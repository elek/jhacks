---
creationDate        : 2005-04-22 17:34:04 +0200 
author              : admin 
title               : j4sql/javadoc tags/j4sql.trigger 
name                : j4sql/javadoc tags/j4sql.trigger 
layout              : wiki 
path                : j4sql/javadoc tags/j4sql.trigger 
date                : 2006-03-26 01:48:07 +0100 
version             : 1 
creator             : kocka 
---
A triggerket ketfelekeppen lehet deklaralni:
a. gyors es megszokott megoldas: nem definialunk neki kulon funkciot, hanem a definialt funkcio csak a triggerhez szolgal
a. definialunk egy funkciot, es arra akarhany triggert is tehetunk.

Pelda1:
```

...
/**
 * Egy eleg extrem eset, tobb trigger ugyanarra a metodusra.
 * 
 * @j4sql.function name="ize_trig_fn"
 * @j4sql.trigger name="ize_trig1" 
 * @j4sql.trigger name="ize_trig2" 
 * 
 */
public static void doInsertEvent(){

}

```
