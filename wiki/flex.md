---
creationDate: 1184763129260 
author: kocka 
contentAuthor: kocka 
title: Flex 
contentUpdateDate: 1212158190513 
name: flex 
layout: wiki 
date: 1212158190513 
creator: kocka 
---
Egy [adobe](adobe.html) (gonosz) cucc, [flash](flash.html) UI generálására. Mivel [java](java.html)-ban lett megírva, platformfüggetlen, az SDK pedig ingyért van. A forráskód (mxml) sima [XML](XML.html) formátumú, helyenként actionscript kód blokkokkal tarkítva a képet :) Tulajdonképpen nem okozhat nagy megdöbbenést azoknak akik gyakran néznek [HTML](Missing.html) vagy [OpenLaszlo](Laszlo.html) kódot.

# [IDE](IDE.html) support

Választási lehetőségek:

 * UI editor hozzá a flex builder, ami [eclipse](Eclipse.html) alapú, viszont sajnos arany árban mérik. Tulajdonképpen a [ide/code completion](ide/code%20completion.html)on kívül nem is tud sokat, azt meg jobbára egy plén [eclipse](Eclipse.html) [XML](XML.html) editorral is meg lehetne oldani ha lenne XSD vagy DTD hozzá. Eddig még nem találtam...
 * Van még egy [payware cucc](http://www.spket.com/download.html) is, ez támogatja az [openalaszlot](Laszlo.html) is.
 * [kocka/flexclipse](kocka/flexclipse.html) by [kocka](kocka.html) - szóval csak bátraknak :) teljesen minimalista

# Features

Remoting: Lehet benne sima [web services](WebServices.html) hívásokkal is dolgozni, vagy [XML](XML.html)+[http](HTTP.html) remoting, esetleg [AMF](AMF.html) protokollal. Open Source backendek mögé a [blazeds](BlazeDS.html) és a [graniteds](Missing.html).
[data binding](data%20binding.html): kapcsos zárójelek közé írt propertynevekkel egyszerűen. Ezzel érdemes eljátszogatni, mert mókás :)

Egy kis demo, csak az ize kedveert...

![image](http://flexclipse.googlecode.com/svn/wiki/editor.jpg)

![image](http://flexclipse.googlecode.com/svn/wiki/swfviewer.jpg)

# Konkurencia

Hasonló termék az [openlaszlo](Laszlo.html), valamennyire az [XML](XML.html) hierarchia is hasnolít, csak ott valami [javascript](javascript.html)-szerű nyelv van, itt meg actionscript ugye. Valamint a flex-ben nem találom (bár nem is hiányzik egyelőre) a proxyzott webapp felállást.

# Tesztelés

[Teszt](test.html) megoldások hozzá:

*   [airRunner](http://airrunner.org)
*   [flexunit](http://code.google.com/p/as3flexunitlib)

# Linkek


*   [Buildelés Mavennel](http://techpolesen.blogspot.com/2007/05/flash-for-java-programmers-lesson-1.html) Mókás kis cucc, sajna a kommentekkel egyet kell értsek: mocsok lassú. Ez van :) [maven/maven2](maven/maven2.html) plugin [itt](http://mvnrepository.com/artifact/net.israfil.mojo/maven-flex2-plugin)
*   Flex 3-hoz [maven](maven/maven2.html) plugin: [itt](http://code.google.com/p/flex-mojos/)
*   [Flex 2.0 @ Work in combination with Spring and Hibernate](http://www.parleys.com/display/PARLEYS/Flex+2.0+at+Work+in+combination+with+Spring+and+Hibernate?showComments=true)
*   [Video Tutorial: Creating an expressive application using Flex, Hibernate, and XFire](http://www.adobe.com/devnet/flex/articles/flexjava.html)
*   [flex.org](http://flex.org/) Flexes komponensek, doksik, ilyesmi...
*   [Rich Text Editor](http://weblogs.macromedia.com/mc/archives/2006/09/disclosable_con_1.cfm)  olyasmi mint az FCKEditor javascriptben.
*   [Top 5 Ways to Reduce Flex Application Startup Time](http://www.infoq.com/news/2008/05/flex-startup-time)
*   [maven](maven.html) repo hozza: [flex mojo](http://flex-mojos.googlecode.com/svn/trunk/repository/)




