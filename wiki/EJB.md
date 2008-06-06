---
creationDate        : 2004-07-27 17:28:47 +0200 
author              : karenin 
title               : EJB 
name                : EJB 
layout              : wiki 
path                : EJB 
date                : 2008-06-06 18:57:03 +0200 
version             : 12 
creator             : zsoltk 
---

-   [EJB2](EJB2.html)
-   [EJB3](EJB3.html)
-   [EJBCA](EJBCA.html)
-   [EJB/entity bean](EJB/entity bean.html)
-   [EJB/MDB](EJB/MDB.html)
-   [EJB](EJB.html)



TODO: elkezdtem átírni EJB3 kompatibilis megállapításokra, sajnos sok mindent kitöröltem emiatt. Közbe viszont rohannom kell, de majd folytatom.

# A varazsszo.

Mielőtt elrettennél a használatától: A következő bekezdések jórészt az EJB2-re vonatkoznak. Azóta megjelent az [EJB 3](Missing.html), ami visszafelé kompatibilis az EJB2-vel és jóval kényelmesebb a használata. A [J2EE](j2ee.html) (manapság Java EE) specifikáció gyüjtemény egy reprezentás tagja).

Tulajdonképpen egy alkalmazásfejlesztő keretrendszer, tipikusan az üzleti logika implementására. Ahogy neve is mutatja Bean-ek családjáról szól. Ezek lehetnek:

Session beanek: ezekbe kerül az üzleti logika. Lehet Stateless és Statefull. Az utóbbit őgy képzeljük el, mintha a metódusok hívása között nálunk maradna egy Session, és az alapján valamifajta állapotot kapcsolna hozzánk a Bean. Alaphelyzetben a Session beanek kezelik a tranzakviókat (jó sok fajta beállítás van, hogy ha épp nincs tranzakció mit csináljon, és ha van akkor mit), vannak benne mindenféle interceptorok (létrehozás előtt, után meghívandó életciklus függvények), tud időzítést, és persze a beaneknek van állapota is, mivel poolozódnak és ide oda mentegetődnek a rendszerben. (És mindezt szemrebbenés nélkül csinálja clusterezett környezetben is.)

Vannak Entity beanek, vagy entitások. Ez [EJB3](EJB3.html) óta [JPA](JPA.html) néven fut, előtte egy kissé bonyoldalmas megoldás volt rá, ne akard tudni, hogy hogy nézett ki.

És vannak Message Driven Beanek, ami aszinkron üzenetek feldolgozására való (tipikusan JMS).

Az egész szoksásoan becsomagolható valami szabály szeirnt, és deployolható.

2 Történet
Jelenleg az EJB 3.1 van fejlesztés alatt, és az EJB 3 a stabil verzió. Az EJB 2, 2.1-et már csak nagyon legacy rendszerekbe használják. Ez a régi változat, még elég bonyolult volt, mindenféle interfacekkel kellet trükközni, és API-t leszármaztatni, és ezt az egészet még némi bonyolult XML leíró is fűszerezte. Az EJB 3-ra leegyszerűsödött, ahol is a modern trendeknek megfelelően mindenhol POJO-t lehet használni, amit aztán oda vissza lehet annotálni. Szóval használható lett. 

Az viszont fontos, hogy az EJB 2.1-nél a háttérben ugyanaz megy, mint az EJB3-nál, csak a használat lett egyszerűbb, tehát a régi tudás teljesen használható.

Az egyik alternatíva 
Mindenestre sokan eskusznek ra (en is), uh. lassan kijon a [EJB3](EJB3.html) specifikacio, ami ugy tunik, vegre olyan szakaszba lep, hogy nem kell hozza pilotavizsga. Azt viszont el lehet mondani hogy kicsit keson kezdett a fejlesztok utan futni a specifikacio, a legtobben vagy inkab 2 retegu rendszert irnak, vagy olyan alternativ megoldasok fele kanyarodtak mint a [spring](spring.html).


3 EJB 2.1
Ha mégis legacy EJB-kkel van dolgod, akkor egyet erdemes megfogadni. Kezzel neki allni [EJB](EJB.html)-ket csinalni ongyilkossag. Keresss valami tool-t, amivel grafikusan, vagy legalabb annotacio szintjen tudod szerkeszteni a Bean-jeidet. De a legjobb, ha inkább átálsz EJB3-ra.

ilyen tool lehet:

*   Szinte bármelyik modern IDE ([JDeveloper](JDeveloper.html), [NetBeans](Netbeans.html), [Eclipse](Eclipse.html))
*   [Websphgere App dev](Missing.html)
*   eszembe jutott:-) [XDoclet](XDoclet.html)
*   AllFusion Joe: [http://www3.ca.com/Solutions/Product.asp?ID=257](http://www3.ca.com/Solutions/Product.asp?ID=257)
*   UML Open Edition: [http://www.umlopenedition.com/ejb_detailed.htm](http://www.umlopenedition.com/ejb_detailed.htm)
*   vDoclet: [http://vdoclet.sourceforge.net/index.html](http://vdoclet.sourceforge.net/index.html)
*   Nem csak EJB, de az is: [http://www.objecteering.com/packaging_personal_edition.php](http://www.objecteering.com/packaging_personal_edition.php)
*   Nem csak EJB, de...:  [http://forge.objectweb.org/projects/lomboz](http://forge.objectweb.org/projects/lomboz)
*   Igaz csak [weblogic](weblogic.html)-hoz: [http://www.beust.com/cedric/ejbgen/](http://www.beust.com/cedric/ejbgen/)

Egyeb tool:

*   [Oracle](Oracle.html) fele EJB verifier: [http://download-east.oracle.com/otn_hosted_doc/jdeveloper/905/ejb/ejb_averfierrules.html](http://download-east.oracle.com/otn_hosted_doc/jdeveloper/905/ejb/ejb_averfierrules.html)

Viszonylag jók a [J2EE](j2ee.html) tutorial \[23..30](Missing.html) megfelelő fejezeteit. [http://java.sun.com/j2ee/1.4/docs/tutorial/doc/index.html](http://java.sun.com/j2ee/1.4/docs/tutorial/doc/index.html)

A feljovo EJB 3:

*   [http://today.java.net/pub/a/today/2004/08/05/ejbnewlife.html](http://today.java.net/pub/a/today/2004/08/05/ejbnewlife.html)

Erdekessegek:

*   [http://www.javaworld.com/javaworld/jw-12-2000/jw-1215-anyclass.html](http://www.javaworld.com/javaworld/jw-12-2000/jw-1215-anyclass.html)

Site-ok:

*   [http://www.ejbsig.de/](http://www.ejbsig.de/)

Lasd meg: [JNDI](JNDI.html), [persistence](persistence.html), [JDBC](JDBC.html), [J2EE](j2ee.html), [RDBMS](RDBMS.html), [IDE](IDE.html)


