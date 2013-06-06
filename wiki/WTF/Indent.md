---
creationDate        : 2005-04-03 14:11:51 +0200 
author              : admin 
title               : WTF/Indent 
name                : WTF/Indent 
layout              : wiki 
path                : WTF/Indent 
date                : 2006-03-26 01:43:01 +0100 
version             : 1 
creator             : kocka 
---
Indantalas java-ban :)

Nem az a tipikus atomszar, de jot rohogtem rajta. Ez nem vicc, ez eles :) Pont ezert veszelyes.

```
    /**
     * Returns indent string.
     */
    public static String indent(int i) {
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
    }
```
