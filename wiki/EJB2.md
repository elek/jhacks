---
creationDate        : 2008-06-07 11:37:58 +0200 
author              : karenin 
title               : EJB2 
name                : EJB2 
layout              : wiki 
path                : EJB2 
date                : 2008-06-07 11:37:58 +0200 
version             : 1 
creator             : karenin 
---
__Ez az oldal még az [EJB3](EJB3.html)-as idők előtti időből származik, elsősorban historikus okok miatt maradt meg, ha kurrens ifnormációkra vágysz, az [EJB](EJB.html) oldal való neked.__

# A varazsszo.

Mielőtt elrettennél a használatától: A következő bekezdések jórészt az EJB2-re vonatkoznak. Azóta megjelent az EJB 3, ami visszafelé kompatibilis az EJB2-vel és jóval kényelmesebb a használata.

Nyugodtan mondhatjuk ra, annak ellenere, hogy nem tul sokan hasznaljak. De mit is erdemes rola tudni? Azt hiszem a Sun celja az volt, hogy valami olyat hozzon letre, aminek segitsegevel az ember megcsinal egy alkalmazashoz tartozo reszben funkcionalis, reszben adatbazis backendet. Egyszer. Aztan kenye kedve szerint eladogatja mindenfele embernek. Egyebkent erre tulajdonkeppen alkalmas is. Peldaul egy konyvaruhaz funkcionalitasat tokeletesen meg lehet EJB-vel csinalni. Az ember ad hozza egy-ket scriptet. Kesz a DB. Kesz a funkcionalis, adatbazis backend. Mar csak egy layout kell, de erre meg van egy rakat.

Szoval valami ilyesmi lebeghetett szemuk elott, amikor lazas agyukban megfogant a dolog. De meg kell mondani, ezt a szerepet nem nagyon toltotte be. Egyszeruen bonyolult. Ahhoz, hogy az ember egyetlen dolgot csinaljon, kell 8 masik, aztan azt a nyolcat meg be is kell passzirozni egy kelloen bonyolult XML leiroba, aztan remenykedik, hogy normalisan mukodik.

Mindenestre sokan eskusznek ra (en is), uh. lassan kijon a EJB3 specifikacio, ami ugy tunik, vegre olyan szakaszba lep, hogy nem kell hozza pilotavizsga. Azt viszont el lehet mondani hogy kicsit keson kezdett a fejlesztok utan futni a specifikacio, a legtobben vagy inkab 2 retegu rendszert irnak, vagy olyan alternativ megoldasok fele kanyarodtak mint a spring.

Sokat lehetne meg meselni, de az alapokhoz erdemes megnezni a J2EE tutorial (23..30) fejezeteit. [http://java.sun.com/j2ee/1.4/docs/tutorial/doc/index.html](http://java.sun.com/j2ee/1.4/docs/tutorial/doc/index.html)

Ha megsem sikerul semmilyen modon elrettenteni, akkor egyet erdemes megfogadni. Kezzel neki allni EJB-ket csinalni ongyilkossag. Keresss valami tool-t, amivel grafikusan, vagy legalabb annotacio szintjen tudod szerkeszteni a Bean-jeidet.

ilyen tool lehet:

*   JDeveloper
*   Websphgere App dev
*   eszembe jutott:-) XDoclet
*   AllFusion Joe: >>[http://www3.ca.com/Solutions/Product.asp?ID=257](http://www3.ca.com/Solutions/Product.asp?ID=257)
*   UML Open Edition: >>[http://www.umlopenedition.com/ejb_detailed.htm](http://www.umlopenedition.com/ejb_detailed.htm)
*   vDoclet: >>[http://vdoclet.sourceforge.net/index.html](http://vdoclet.sourceforge.net/index.html)
*   Nem csak EJB, de az is: >>[http://www.objecteering.com/packaging_personal_edition.php](http://www.objecteering.com/packaging_personal_edition.php)
*   Nem csak EJB, de...: >>[http://forge.objectweb.org/projects/lomboz](http://forge.objectweb.org/projects/lomboz)
*   Igaz csak weblogic-hoz: >>[http://www.beust.com/cedric/ejbgen/](http://www.beust.com/cedric/ejbgen/)

Egyeb tool:

*   Oracle fele EJB verifier: >>[http://download-east.oracle.com/otn_hosted_doc/jdeveloper/905/ejb/ejb_averfierrules.html](http://download-east.oracle.com/otn_hosted_doc/jdeveloper/905/ejb/ejb_averfierrules.html)

A feljovo EJB 3:

*   [http://today.java.net/pub/a/today/2004/08/05/ejbnewlife.html](http://today.java.net/pub/a/today/2004/08/05/ejbnewlife.html)

Erdekessegek:

*   [http://www.javaworld.com/javaworld/jw-12-2000/jw-1215-anyclass.html](http://www.javaworld.com/javaworld/jw-12-2000/jw-1215-anyclass.html)

Site-ok:

*   [http://www.ejbsig.de/](http://www.ejbsig.de/)

Lasd meg: JNDI, persistence, JDBC, J2EE, RDBMS, IDE
