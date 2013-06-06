---
creationDate        : 2004-07-27 21:25:23 +0200 
author              : kocka 
title               : Aspect Oriented Programming 
name                : AOP 
layout              : wiki 
path                : AOP 
date                : 2006-10-20 13:30:03 +0200 
version             : 9 
creator             : zsoltk 
---
Anno a [Sztupi](sztupi.html) nevezetu emberke hivta fel ra a figyelmemet. Gyakorlatilag legendakat zengett rola, uh. meg is neztem. Elsore nem teljesen lattam at, ertettem meg mire is valo, meg hogyan is erdemes csinalni, de vegul megertettem. (Egy reszet)

A dolog nagyjabol es egeszebn arrol szol, hogy az ember programja egyre atlathatatlanabb lesz, ahogy fejlodik. Szepen megcsinalja a designt, aztan az idok folyaman egyre ujabb es ujabb dolgok tunnek fel, amiket szepen bele kell gyurni a rendszerbe. A vegeredmeny az, hogy a kulonbozo funkcionalitasokhoz tartozo kodreszletek szanaszet szorva lesznek benne a kodban. Ami belethato, hogy eleg nagy akoszhoz fog vezetni egy ido utan.

Ennek a dolognak a kivedesere talaltak ki az AOP-ot.

Tehat az AOP egyik alap koncepcioja az, hogy az ember megirja az [OOP](oop.html) modellt, de ebben csak azokra a dolgokra koncentral, ami a funkcionalitashoz szukseges. Minden egyeb dolog (pld.: [logging](Logging.html)) az aspektusokban tortenik.

Termeszetesen, hogy hol a hatar az OOP modell es az AOP funkcionalitas kozott, meg nem kerult egyertelmuen meghatarozasra es szerintem itt is a jozan esz fog diktalni.

pld.: Irsz egy neuralis halot, amiben a halot reprezentalo objektumok nagyon jol behatarolhato funkcioval birnak. de ugye kene tudni logolni, meg azert kene tudni monitorozni, meg kene tudni grafikusan a kapcsolodo informaciokat megjeleniteni...

Na most itt akkor 2 lehetoges van: vagy interface-k segitsegevel minden, a halo megvalositasahoz tartozo objektumba belegyurod ezeket a funkciokat, vagy aspektusokat (aspect) hasznalsz.

Az elso lehetoseg jarhato, de a kod erosen atlathatatlan lesz, raadasul az eredeti funkcionalitas melle (Neuralis halo) meg egy rakat egyeb is bejon, ami nem igazan tartozik szorosan az NN temakorebe.

A masodik esetben, hagyod a haloobjektumokat ugy ahogy vannak es minden egyeb funkcionalitast aspektusok segitsegevel irsz meg. Mondanom sem kell, hogy ez lenyegesen atlathatobb kodot eredmenyez.

Hogy melyiket valasztod (keves aspect, sok interface vs. keves interface sok aspect) csak rajtad mulik. Mindenestere az AOP levlistan egyre jobban a masodik fele hajlanak az emberek.

A masik lenyeges dolog, amiert az AOP hasznalhato, az az elore nem latott funkcionalitas szuksegessege. Ebben az esetben az ember nagyreszt atgyurja az OOP modellt, hogy a funkcionalitas letrejojjon. Aki csinalt mar ilyet, tudja mire gondolok. De mi van akkor, ha az eredeti [OOP](oop.html) modell modositasa nelkul tudsz uj funkcionalitast adni? Erre is lehetoseg van az AOP-on belul.<br/>

Ha ez a rovid kis ismerteto felkeltette az erdeklodesed, akkor a kovetkezoket ajanlom:

*   A legnagyobb kapcsoloszajt: [http://aosd.net/](http://aosd.net/)
*   [Eclipse](Eclipse.html) AJDT plugin: [http://www.eclipse.org/ajdt/](http://www.eclipse.org/ajdt/)
*   Az [AspectJ](Missing.html) nevezetu project: [http://eclipse.org/aspectj/](http://eclipse.org/aspectj/)
*   Es a hozza tartozo dokumentacio, ami a fenti peldakat eleg jol targyalja: [http://dev.eclipse.org/viewcvs/indextech.cgi/~checkout~/aspectj-home/doc/progguide/index.html](http://dev.eclipse.org/viewcvs/indextech.cgi/~checkout~/aspectj-home/doc/progguide/index.html)

Es igerem, hogy az AOP listat vegig fogom nezni es kiszedegetem azokat a best practice-okat, amiket emberek kitermeltek. Kisdobos szavamra!


__[stoned](stoned.html) irta a kovetkezoket a szocikkhez:__

A klasszikus példa a logger aspect, fejlesztés közben nem kell teleszórni a kódot logger.debug() sorokkal. A unit teszteket is fel lehet tuningolni, illetve egyszerűbbé tenni.

Vannak aztán a production aspectek, amikor nem kell a kódot security management, transaction management concernekkel szennyezni. Az Aspectj in Action könyvben rengeget pattern van.

Kétféle megoldás létezik, az egyik a [bytecode](bytecode.html)-ot módosítja fordításkor vagy futás közben, a másik a proxy alapú megoldások (és persze van amelyik mindkettőt cglibbel vagy javassisttal).

[Bytecode](bytecode.html) módosítók:

[http://eclipse.org/ajdt/](http://eclipse.org/ajdt/) : [AspectJ](Missing.html). Az első Javas aspect megvalósítás AFAIK. A java szintakszis kibővítése, saját fordítóval, ami fordításkor "weaveli" össze az aspecteket (Az új verzióban mintha lenne valami runtime lehetőség is, de nem vagyok benne biztos). Az eclipse integrációnak köszönhetően remek tool support. Ő a "nagyágyú". (spring integráció folyamatban van).

[http://aspectwerkz.codehaus.org](http://aspectwerkz.codehaus.org) : Fordításkori és runtime bytecode módosítással éri el a célját. Elég flexibilis megoldás, marad a java szintakszisnál, xml-ben vagy java kóddal lehet konfigurálni. Ha jól emlékszem classloaderekkel oldja meg amit kell.

Proxy alapú frameworkök:

[http://jboss.org/products/aop](http://jboss.org/products/aop) : Erről keveset tudok, a [JBoss](jboss.html) 4.0 része lesz, bár úgy tudom, általános megoldásnak is szánják. AFAIK a Javassistot használja, szóval lehet hogy nem is proxy alapú? :-)

[http://dynaop.dev.java.net/](http://dynaop.dev.java.net/) : dynaop. Lightweight aop implementáció, dynamic proxy-t vagy [cglib](Missing.html)et használ. [BeanShell](BeanShell.html) konfiguráció. Igen gyors. Nekem nagyon tetszik :-) Támogatja az [http://aopalliance.sourceforge.net/](http://aopalliance.sourceforge.net/) APIt.

[http://springframework.org](http://springframework.org) : [Spring](spring.html) framework AOP implementációja. Konténerspecifikus megoldás, a fejlesztők nem is ajánlják általános felhasználásra. Rengeteg hasznos dolgot lehet csinálni vele a frameworkben (deklaratív security, deklaratív transaction management, stb). Szintén támogatja az [http://aopalliance.sourceforge.net/](http://aopalliance.sourceforge.net/) APIt.

[http://nanning.codehaus.org](http://nanning.codehaus.org) : Leightwieght megoldás, erős [picocontainer](picocontainer.html) integrációval. Abszolút nem ismerem…
