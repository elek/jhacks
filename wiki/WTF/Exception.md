---
creationDate        : 2005-04-18 12:18:52 +0200 
author              : admin 
title               : WTF/Exception 
name                : WTF/Exception 
layout              : wiki 
path                : WTF/Exception 
date                : 2006-03-26 01:43:01 +0100 
version             : 1 
creator             : kocka 
---
Megoldas az exception okanak titokban tartasara.

```

    try {
      ize = hello();
    } catch (Exception ex) {
      if (ex.getMessage() != null)
        throw new RuntimeException(e.getMessage());
      throw new RuntimeException();
    }
```

Az hogy mi lehetett az oka az ilyen nehezen emesztheto hibakezelesnek, [itt](http://c2.com/cgi/wiki?ThrowsExceptionByDefault) irja le egy cikk, utanna azt is leirjak hogy miert hibas.
