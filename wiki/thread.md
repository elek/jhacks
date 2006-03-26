---
creationDate        : 2005-04-11 10:52:40 +0200 
author              : admin 
title               : thread 
name                : thread 
layout              : wiki 
path                : thread 
date                : 2006-03-26 01:51:18 +0100 
version             : 1 
creator             : kocka 
---
Lasd: [java.lang.Thread](http://docs.oracle.com/javase/7/docs/api/java/lang/Thread.html)

A [java](java.html) a szintaxisaba foglalta a tobbszalusagot tamogato konstrukciokat, ezzel sokkal konnyebbe es biztonsagosabba tette a tobbszalu programozast. Persze voltak kezdeti hibak, ilyen volt a thread stop metodusa, amit aztan [deprecated](deprecated.html)de tettek.

Erdemes megismerkedni a [synchronized](Missing.html) kulcsszoval, ami meggatolja hogy egy kritikus zonaba egyszerre ket programvegrehajtasi szal lepjen be. Kombinalva ezt az [exception](Missing.html) kezelessel, egy egesz biztonsagos dolgot kapunk.

```

...
try{
  synchronized (this) {
    //kritikus szakasz
  }
} finally {
  //satobbi
}

```

Szoval a kiraj benne az, hogy a kritikus szakaszban ha valami hiba tortenik, akar olyan amire nem volta a programozo felkeszulve, a lock akkor is feloldodik, es a kovetkezo szal belephet a blokkba, es ezt a [JRE](JRE.html) garantalja.
