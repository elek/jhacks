---
creationDate        : 2005-07-18 23:21:27 +0200 
author              : karenin 
title               : Document Object Model 
name                : dom 
layout              : wiki 
path                : dom 
date                : 2007-06-14 13:09:04 +0200 
version             : 2 
creator             : kocka 
---
Az [xml](XML.html) strukturak nyelvfuggetlen reprezentacioja. Sajnos nem passzol tul jol a [java](java.html)hoz (a nyelvfuggetlenseg atka), ezert az alapm JVM tartalmat implementacio sem epul a collections frameworkre, eleg nehezkesen hasznalhato.
Ha DOM kell neked, akkor nezd meg elotte a [dom4j](dom4j.html) es [JDom](jdom.html) alkalmazasokat (főleg az utóbbit), amik szinten kompatibilisek a szabvanyos DOM modellel, de ok tudnak sok okosabb dolgokat (pl. Collection kezeles).
A DOM alapbol berantja a az egesz XML fajlt a memoriaban, ezert nagy/sok fajlnal kevesbe hatekony. Ilyenkor hasznald a [SAX](sax.html)-ot vagy meg inkabb a [StAX](StAX.html)  [xml](XML.html) apikat. Amugy beolvasashoz/parzolashoz altalaban a DOM megvalosiatsok is a [sax](sax.html)ot hasznaljak.

Valami ilyesmi:
```
DocumentBuilderFactory factory = DocumentBuilderFactory.newInstance();
DocumentBuilder builder = factory.newDocumentBuilder();
Document document = builder.parse(inputStream);
NodeList nodes = document.getElementsByTagName("sampletag");
if (nodes.getLength()!=0) Node foo = nodes.item(0);
```
