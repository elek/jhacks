---
creationDate        : 2005-04-03 14:11:51 +0200 
author              : kocka 
title               : WTF/Indent 
name                : WTF/Indent 
layout              : wiki 
path                : WTF/Indent 
date                : 2005-04-03 14:14:45 +0200 
version             : 2 
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
