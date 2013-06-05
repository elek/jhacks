---
creationDate: 1091464825212 
author: kocka 
contentAuthor: kocka 
title: tapestry 
contentUpdateDate: 1159782016010 
name: tapestry 
layout: wiki 
date: 1159782016010 
creator: stoned 
---
http://jakarta.apache.org/tapestry

__faj__: java alapú web framework (lásd még [struts](struts.html), [webwork2](Missing.html), http://waferproject.org )

__alfaj__: komponens alapú web framework (mint pl. [jsf](JSF.html))

__jellemzők__: Szakítás a hagyományos [MVC](MVC.html) paradigmával, komponens alapú fejlesztésre helyezve a hangsúlyt. Eltérően a hagyományos MVC-vel, az alkalmazás fejlesztőjének nem kell törődnie az URL paraméterekkel, a Session objecttel, úgy általában a [Servlet](servlet.html) API-val (Természetesen ettől függetlenül lehetőség van az API elérésére). Ennek következtében az evolúció ezen szakaszában a framework által generált URL-ek nem túl kereső- és bookmark barátok, de ez a közeljövőben változni fog, és egyébként is van workaround.

Sok ötletet merít az Apple féle [WebObjects](Missing.html) nevű projektből, így akik azt ismerik, a Tapestry-t is ismerősnek találják majd.

A rugalmas felépítésnek köszönhetően rengeteg előnnyel rendelkezik a többi fajhoz képest:
* Parameter binding. A framework automatikusan bindingeli (hunglish rulez again) a request parametereket a fejlesztő által írt [java](java.html) osztályok property-jeihez. Ehhez kapcsolódik egy nagyon király validation facility, ahol magát a validáció logikáját is meghatározhatjuk (ha nem elég az a pár default validation bean, amit már születéskor tartalmaz a szervezet), csakúgy, mint a tüneteket (look & feel).
* Session handling. Lehetőség van a "régimódi" session kezelésre, azaz a session objektumban eltárolni a session adatait, de köszönhetően a persistent component property-knek, a tökölés a sessionnel nagyban lecsökkenthető. A persistent component property azt jelenti, hogy minden komponens deklarálhat property-ket, amik ha persistentként vannak deklarálva, a framework gondoskodik arról, hogy a session során ezek megőrizzék értéküket. Ennek köszönhetően a hosszútávú memóriában észlelhető zavarok is csökkenthetőek.
* Valid HTML templates. A bestia külső felépítése nagyban megkönnyíti a fodrászok, mani- és pedikűrösök, esetleg plasztikai sebészek munkáját. A Tapestry template-ek érvényes (X)HTML file-ok, amit egy mezei, Java-hoz, tag library-khez mit sem értő web designer is könnyen elkészíthet, sőt, az operáció előtt lehetőség van a végeredmény azonnali tesztelésére html böngészők segítségével.
* High level of reuse. Már születéskor tartalmazza a fejlesztéshez [elengedhetetlen komponenseket](http://jakarta.apache.org/tapestry/doc/ComponentReference/index.html) (framework library), egyéb hasznos komponenseket (contrib library), és még wml komponenseket is (wml library). Saját library-k készítése és felhasználása gyerekjáték. Ezek fejlesztése (legjobb tudomásom szerint) jóval egyszerűbb, mint a [JSP](JSP.html) tag-libraryk fejlesztése.
* Line precise error reporting. Ez kemény. Ha beteg megmondja hol fáj, mi fáj, és még a vércsoportját is közli. Najó, kicsit kevésbé elvontan tartalmaz egy komponenst a framework, ami megjelenít minden információt egy el nem kapott kivétel esetén. Erősen addiktív feature. [példa kórlap](http://www.t-deli.com/workbench/app?service=page/ErrorFest) .
* Dokumentáció. Sokáig nagy hibája volt a fajnak, hogy belső felépítését csak néhány beavatott, igen képzett kutató ismerte. Az kutatáshoz újonnan hozzákezdő zöldfülűeknek nagy gondot okozott a megszokott [MVC](MVC.html) arhitektúráktől eltérő fejlesztési model. Szerencsére manapság sokkal több információ áll rendelkezésre a lelkes fejlesztők számára. A cikk végén felsorolásra kerülnek a lelőhelyek is. A dokumentációkon kívül - jó opensource hagyományokhoz híven - a levelező lista igen segítőkész és hatékony.
* [IDE](IDE.html) support (Csak [eclipse](Eclipse.html) egyelőre, de hát az A [java](java.html) [ide](IDE.html) nem? ;-)). Bár Tapestry alkalmazások könnyedén fejleszthetők egy pőre [vim](VIM.html) segítségével is, de a http://spindle.sourceforge.net project sok-sok unalmas gépeléstől és hibakereséstől mentesíti a fejlesztőt. A spindle alkotója szerencsére nem esett abba a hibába, hogy egy WYSIWYG típúsu szörnyet készítsen. Ehelyett code completion, egy-két wizard található benne, és egy saját builder, ami képes (elvileg) minden hibát észlelni a html template-ekben és component descriptorokban.

Számos előnye mellett néhány hátránnyal is rendelkezik a faj, amik elsőrorban szociális problémák (lassan múló beilleszkedési zavarok):
* Learning curve. A hagyományos [MVC](MVC.html)-hez szokott fejlesztőknek eltarthat egy darabig, amíg hozzászoknak az inkább a swinghez, mintsem a Model2 MVC-hez hasonló fejlesztési modelhez.
* Nem mainstream. A [Struts](struts.html) mellett nehezen jut szóhoz. A struts gyakorlatilag a szabvány [J2EE](j2ee.html) view layer technológia. Mint általában a szabványoknál, nem feltétlenül a legfejlettebb megoldás, de sokan használják.
* A [SUN](Sun.html) helyett az apache áll mögötte. Nem rossz társaság az apache group (bár vannak furcsa szokásaik), mégsem olyan erőteljes szervezet, mint a [SUN](Sun.html). A [SUN](Sun.html) mostanában kezdi erőltetni a [JSF](JSF.html) nevű új technológiáját, ami elmondások szerint egy a tapestry-hez hasonló szörnyeteg, de igazi developer toolok nélkül esélytelen a fejlesztés JSF-el. Mivel erős lobbi áll mögötte ([SUN](Sun.html) és más tool developers) várhatóan jobban elterjed majd, mint a kis Tapestry :-(

Néhány lelőhely bővebb információkra éhezőknek:
* [komponens dokumentáció](http://jakarta.apache.org/tapestry/doc/ComponentReference/index.html)
* [Wiki](http://wiki.apache.org/jakarta-tapestry/)
* [Introduction to Jakarta Tapestry by OCI](http://www.ociweb.com/jnb/jnbMay2004.html)
* [Tutorial by Kevin C. Dorf](http://dorffweb.com/?page=taptutorial)
* [Még egy remek tutorial](http://www.sandcastsoftware.com/articlesandtutorials/brownbag/)
* [Tapestry integráció a springframeworkbe](http://www.springframework.org/docs/reference/view.html#view-tapestry)
* [Tapestry in Action](http://www.manning.com/lewisship/) Ez a könyv a framework szerzőjének könyve, megéri meg..hmm..szerezni ;-) Egyébként megéri a pénzt.
* http://spindle.sourceforge.net tapestry plugin eclipse-hez
* http://jroller.com/page/glongman/ spindle alkotójának weblogja. Érdemes az unstable-t kipróbálni (és használni!), itt jelennek meg a hírek az újabb unstable releasről.

Minta alkalmazások:
* [Tapestry+Hibernate](http://nemesisit.rdsnet.ro/opendocs/tapehibe2/tapehibe2.html)
* [Better petshop (Spring+Tapestry+Hibernate)](https://betterpetshop.dev.java.net/)
* [Workbench](http://www.t-deli.com/workbench/app) Működő demó néhány Tapestry feature demonstrálására. Dates, chart, exception: lotta fun. Pallette: ez kérem egy komponens a contrib library-ből. És ahh. A jobb alsó sarok. Inspector komponens.


