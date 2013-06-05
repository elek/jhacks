---
creationDate: 1120853415793 
author: karenin 
contentAuthor: karenin 
title: Java Businness Integration 
contentUpdateDate: 1180446480699 
name: JBI 
layout: wiki 
date: 1180446480699 
creator: kocka 
---
Egy [JSR](JSR.html) uzleti integracohoz. Eleg uj es egyelore nem fog elterjedni szelesebb korben. Peldaul azert mert a gagyi [w3c](w3c.html) dom apit hasznalja ami gebaszos.

Tulajdonkép az [ESB](ESB.html) tervezési mintának egy Javaban írt (szabványos) implementációja. A váza elég egyszerű van egy ESB, amit Normalized Message Routernek hívnak, és azon keresztül hívogatják egymás a komponenesek. Komponesn kétféle van: Binding Component (BC) és Service Component (SC). Ezek mindegyike a Message Bus/Router felé [webservices](WebServices.html)-nek látszanak. 

A BC-k ezen kívül egy másik oldalról is láthatóak egyéb specifikus specifikus protokolokon keresztül (Azaz az SMTP BC pl. egy SMTP-re jövő emailt tud átfordítani a Message Router-en közlekedő WebService hívássá vagy fordítva).

Az SC-k mindkét felükkel (input/output) a Message Router-en csücsülnek, és sokszor valami tartalmat is lehet beléjük deployolni (pl. XSLT transzformáló SC-be egy konkrét XSLT-t).

Bár elvileg a Routeren keresztül mindenhol WebService hívások mennek, annyire nem vészes a helyzet, mert a busz tudja, ha Java-ból Java-t hív és szépen kioptimalizálja.

A speckó javára lehet még írni, hogy a managementet is pontosan definiálja (nem úgy mint az [EJB](EJB.html)-knél) JMX és ANT task szinteken.


Linkek:

*   http://www.jcp.org/en/jsr/detail?id=208



Implementaciok:
*   [servicemix](servicemix.html)
*   [mule](mule.html)
*   [celtix](celtix.html)
*   [OpenESB](OpenESB.html)



Lasd meg: [JMS](JMS.html), [ESB](ESB.html)
