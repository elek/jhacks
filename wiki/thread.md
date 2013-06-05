---
creationDate: 1113209560514 
author: kocka 
contentAuthor: kocka 
title: thread 
contentUpdateDate: 1113209560514 
name: thread 
layout: wiki 
date: 1113209560514 
creator: kocka 
---
Lasd: 

A [java](java.html) a szintaxisaba foglalta a tobbszalusagot tamogato konstrukciokat, ezzel sokkal konnyebbe es biztonsagosabba tette a tobbszalu programozast. Persze voltak kezdeti hibak, ilyen volt a thread stop metodusa, amit aztan [deprecated](deprecated.html)de tettek.

Erdemes megismerkedni a [synchronized](Missing.html) kulcsszoval, ami meggatolja hogy egy kritikus zonaba egyszerre ket programvegrehajtasi szal lepjen be. Kombinalva ezt az [exception](Missing.html) kezelessel, egy egesz biztonsagos dolgot kapunk.

{% highlight java %}

...
try\{
  synchronized (this) \{
    //kritikus szakasz
  \}
\} finally \{
  //satobbi
\}

{% endhighlight %}

Szoval a kiraj benne az, hogy a kritikus szakaszban ha valami hiba tortenik, akar olyan amire nem volta a programozo felkeszulve, a lock akkor is feloldodik, es a kovetkezo szal belephet a blokkba, es ezt a [JRE](JRE.html) garantalja.
