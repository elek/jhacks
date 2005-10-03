---
creationDate        : 2005-10-03 15:17:23 +0200 
author              : suhaig 
title               : WTF/Unsupported constructor 
name                : WTF/Unsupported constructor 
layout              : wiki 
path                : WTF/Unsupported constructor 
date                : 2005-10-03 15:17:23 +0200 
version             : 1 
creator             : suhaig 
---
Valaki esetleg megmagyarazhatna, koszonom.
<br/>
```
private ValamiClass() throws java.lang.UnsupportedOperationException {
    throw new java.lang.UnsupportedOperationException("Illegal constructor call");
}
```
