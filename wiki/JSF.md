---
creationDate: 1159046533334 
author: kocka 
contentAuthor: kocka 
title: JSF 
contentUpdateDate: 1212938204034 
name: JSF 
layout: wiki 
date: 1212938204034 
creator: karenin 
---
Java Server Faces (jsr 127). Webes framework. Sokan a [Struts](struts.html) utodjanak mondjak, mert a vezetoje az a bizonzos Craig McClanahan, aki a [Struts](struts.html)-ert is felelos.

Alapvetoen [servlet](servlet.html)-ek melle egy lib + tag library. A web oldalakat  komponens fában képzeli el (mint mondjuk egy hagyomanyos [GUI](gui.html) pl. a [Swing](Swing.html)). A komponensek sajat maguk importaljak a bejovok requestbol az erteket, validaljak, es renderelik magukat. A komponenes fat tipikusan [jsp](JSP.html)-ben definialjuk, amikben jsf tag librarykkal definialjuk az elemeket.

E mellett meg van melle egy rakas beanunk is kulonbozo scope-pal (page, request, session...) Amit EL szeru nyelvvel szepen ra bindelunk a jsp fajlban a fa strukturankra. (A beanek melyik eleme melyik komponensnek adja az erteket)

Az egesz ugy megy, hogy a web.xml-be beirjuk a JSF Front Controlleret es onnantol kezdve az url-eknel o nez utana, hogy van-e hozza jsf szeru [jsp](JSP.html). Tud okos validatorokat es convertereket is (amit persze a Spring is, de a Struts asszem nem tudott), hogy a bean-ekbe milyen tipusokka kepzodjenek le a bemeneti String request elemek.

A JSF rajongoinak egy resze azert lelkesedik, hogy milyen jo WYSIWYG szerkesztoket lehet csinalni, ahol vizualisan dobalgatjuk bele a komponenseket az oldalba es ott kotogetjuk ossze oket. Ez szep dolog, de ahogy en tudom ez a resze a JSF-nek meg nem szabvanyos (marmint az, hogy a komponensbe beleird, hogy visual szerkeszto eseten mit mutasson,  es mit lehessen rajta beallitani). Azaz ez mind csak Sun Java Studio Creator specifikus. 

Masok ezt a lelkesedest eleg ketkedve figyelik.

Amugy eleg izgalmas dolog, elso sorban formok feldolgozasaban jo, meg egy szabvanyos felulet arra, hogy ujrahasznosithato okos komponenseket fejlesszunk (pl. [AJAX](ajax.html)-os beviteli elemek).

Egyéb: [seam](Missing.html)

Linkek:

*   [Basics and Concepts of JSF](http://parleys.com/display/PARLEYS/Basics+and+Concepts+of+JSF?showComments=true)




