---
creationDate: 1100515480473 
author: kocka 
contentAuthor: kocka 
title: beehive 
contentUpdateDate: 1129553451661 
name: beehive 
layout: wiki 
date: 1129553451661 
creator: boci 
---
[__Apache Beehive__](http://beehive.apache.org/)

Ez a Project az [Apache](http://www.apache.org) zaszloja alatt egy [J2EE](j2ee.html) es a [Struts](struts.html) otvozeset tuzte ki celul. A lapok kapcsolatait Flow diagrammon keresztul adhatjuk meg. Jelenleg inkubator allapotban leledzik (Alpha V1) de igen figyelemremelto.

[Eclipse](Eclipse.html)-hez keszult mar hozza egy [pollinate](pollinate.html) nevu editor plugin, ami nem mellesleg az Eclipse Technology Project egisze alatt fut, tehat nem valami kis csoport altal fejlesztett kulso plugin.

Az alapgondolata valami olyasmi hogy Contol-okat hozol letre, ezeket az actionok parameterezik fel es adjak at a [jsp](JSP.html)-nek. Szoval a [jsp](JSP.html) egyszeruen felhasznalhatja ezeket, es nem kell bele java kodot irni.

A masik dolga a page flow, ami egy kicsit kodos hogy hogy muxik :)

De mindenesetre mindezt [java 1.5](java%201.5.html) [annotations](annotations.html) supporttal teszi.

<[kocka](kocka.html)-comments>

Egy ket dolog amit nem ertek benne.

*   Miert kell a Controller.java-t pont a jsp-k koze tenni?
*   Miert olyan nagy dolog az hogy olyan dolgokat amit ugy is mindenki tud ([ejb](EJB.html), [jdbc](JDBC.html), [jms](JMS.html)) controllerek moge tettek? Meg igy is eleg konkretak.
*   mi a turo az a specialis [ant](ant.html) task? Miert nem lehet csak ugy a szokasos modon buildelni?
*   Minek masni a nyers husokra?



Egyebkent ha egyszer kesz lesz a [pollinate](pollinate.html), akkor biztos franko lesz, de tegnapra legyen mar kesz :)

</[kocka](kocka.html)-comments>
