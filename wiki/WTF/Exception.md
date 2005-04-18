---
creationDate        : 2005-04-18 12:18:52 +0200 
author              : kocka 
title               : WTF/Exception 
name                : WTF/Exception 
layout              : wiki 
path                : WTF/Exception 
date                : 2005-04-18 13:35:36 +0200 
version             : 4 
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
