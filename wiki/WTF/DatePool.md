---
creationDate        : 2005-04-04 12:05:39 +0200 
author              : admin 
title               : WTF/DatePool 
name                : WTF/DatePool 
layout              : wiki 
path                : WTF/DatePool 
date                : 2006-03-26 01:43:01 +0100 
version             : 1 
creator             : renszarv 
---
Már nem production kód, de az volt (emlékezetből, csak a lényeg)

```

 private static int datePos = 0;
private static Date[] datePool = new Date[16];


 public static String toString(long time) {
     Date date = datePool[datePos++ % datePool.length];
     date.setTime(time);
     return date.toString();
 }
```

 Persze bármilyen szinkronizáció nélkül ... 
