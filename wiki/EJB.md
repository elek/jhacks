---
creationDate        : 2004-07-27 17:28:47 +0200 
author              : kocka 
title               : EJB 
name                : EJB 
layout              : wiki 
path                : EJB 
date                : 2007-08-21 17:38:52 +0200 
version             : 9 
creator             : zsoltk 
---

-   [EJB2](EJB2.html)
-   [EJB3](EJB3.html)
-   [EJBCA](EJBCA.html)
-   [EJB/entity bean](EJB/entity bean.html)
-   [EJB/MDB](EJB/MDB.html)
-   [EJB](EJB.html)



# A varazsszo.

Nyugodtan mondhatjuk ra, annak ellenere, hogy nem tul sokan hasznaljak. De mit is erdemes rola tudni? Azt hiszem a [Sun](Sun.html) celja az volt, hogy valami olyat hozzon letre, aminek segitsegevel az ember megcsinal egy alkalmazashoz tartozo reszben funkcionalis, reszben adatbazis backendet. Egyszer. Aztan kenye kedve szerint eladogatja mindenfele embernek. Egyebkent erre tulajdonkeppen alkalmas is. Peldaul egy konyvaruhaz funkcionalitasat tokeletesen meg lehet [EJB](EJB.html)-vel csinalni. Az ember ad hozza egy-ket scriptet. Kesz a DB. Kesz a funkcionalis, adatbazis backend. Mar csak egy layout kell, de erre meg van egy rakat.

Szoval valami ilyesmi lebeghetett szemuk elott, amikor lazas agyukban megfogant a dolog. De meg kell mondani, ezt a szerepet nem nagyon toltotte be. Egyszeruen bonyolult. Ahhoz, hogy az ember egyetlen dolgot csinaljon, kell 8 masik, aztan azt a nyolcat meg be is kell passzirozni egy kelloen bonyolult XML leiroba, aztan remenykedik, hogy normalisan mukodik.

Mindenestre sokan eskusznek ra (en is), uh. lassan kijon a [EJB3](EJB3.html) specifikacio, ami ugy tunik, vegre olyan szakaszba lep, hogy nem kell hozza pilotavizsga. Azt viszont el lehet mondani hogy kicsit keson kezdett a fejlesztok utan futni a specifikacio, a legtobben vagy inkab 2 retegu rendszert irnak, vagy olyan alternativ megoldasok fele kanyarodtak mint a [spring](spring.html).

Sokat lehetne meg meselni, de az alapokhoz erdemes megnezni a [J2EE](j2ee.html) tutorial \[23..30](Missing.html) fejezeteit. [http://java.sun.com/j2ee/1.4/docs/tutorial/doc/index.html](http://java.sun.com/j2ee/1.4/docs/tutorial/doc/index.html)

Ha megsem sikerul semmilyen modon elrettenteni, akkor egyet erdemes megfogadni. Kezzel neki allni [EJB](EJB.html)-ket csinalni ongyilkossag. Keresss valami tool-t, amivel grafikusan, vagy legalabb annotacio szintjen tudod szerkeszteni a Bean-jeidet.

ilyen tool lehet:

*   [JDeveloper](JDeveloper.html)
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

A feljovo EJB 3:

*   [http://today.java.net/pub/a/today/2004/08/05/ejbnewlife.html](http://today.java.net/pub/a/today/2004/08/05/ejbnewlife.html)

Erdekessegek:

*   [http://www.javaworld.com/javaworld/jw-12-2000/jw-1215-anyclass.html](http://www.javaworld.com/javaworld/jw-12-2000/jw-1215-anyclass.html)

Site-ok:

*   [http://www.ejbsig.de/](http://www.ejbsig.de/)

Lasd meg: [JNDI](JNDI.html), [persistence](persistence.html), [JDBC](JDBC.html), [J2EE](j2ee.html), [RDBMS](RDBMS.html), [IDE](IDE.html)


