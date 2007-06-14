---
creationDate        : 2007-06-14 13:15:42 +0200 
author              : karenin 
title               : StAX 
name                : StAX 
layout              : wiki 
path                : StAX 
date                : 2007-06-14 13:16:19 +0200 
version             : 2 
creator             : karenin 
---
Pull parser Java-hoz. Keveset eszik (mint a [Sax](sax.html)) de nem a parser dirigálja az event függvényt, hanem mindig parser.next()-et kell mondani, ha szeretnéd a következő tokent. Ezért aztán nagyon jó, ha az XML csak egy része érdekel, mert könnyű kiszálnni/skip-elni a többi tagnál.
Egy konkret esetben nekem a [sax](sax.html)-nal is gyorsabbnak bizonyult egy 50-60%-kal.

Java EE 5-ben alapbol benne van, ha 1.4-esed van, akkor gyorsan frissits :).

Az illata:
```
XMLInputFactory f = XMLInputFactory.newInstance();
XMLStreamReader r = f.createXMLStreamReader(inputStream);
while(r.hasNext()) {
  if (r.getEventType()==XMLStreamConstants.START_ELEMENT){
    if ("sampletag".equals(r.getLocalName())) {
      System.out.println("bingo");
      //a tobbi reszt mar nem dolgozzuk fel.
      break;
    }
  }
r.next();
```
