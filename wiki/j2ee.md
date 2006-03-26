---
creationDate        : 2004-07-28 14:32:48 +0200 
author              : admin 
title               : J2EE 
name                : j2ee 
layout              : wiki 
path                : j2ee 
date                : 2006-03-26 01:48:04 +0100 
version             : 1 
creator             : zsoltk 
---
![image](http://hackers.forgeahead.hu/space/SnipSnap/config/j2ee_jdk_button_classic_red.gif)(http://java.sun.com/j2ee/download.html)

Java 2 Enterprise Edition.

# Bevezeto

A J2EE a [java](java.html) programozasi nyelv szerveroldali felhasznalasat celzo APIk gyujtemenye, azaz olyan dolgok amik foleg ceges felhasznalasra lettek kitalalva. A J2EE tervezoi egy tobbretegu hierarchiat almodtak meg, ami az [EJB](EJB.html), [JCA](JCA.html), [servlet](servlet.html), [jsp](JSP.html) reszekbol allt nagyjabol, amit igazabol azt hiszem eleg kevesen vetettek be. Ugyanis eleg sok uj dolgot kellett volna megtanulni, bar ezt szet lehetett volna bontani a [j2ee development roles](j2ee%20development%20roles.html) szerint, de a gyakorlatban azt lattuk hogy valami miatt megsem tortent igy. Igy aztan szuletett mindenfele, a stack bizonyos reszet helyettesito megoldas ([spring](spring.html), [struts](struts.html), [tapestry](tapestry.html), [hibernate](Hibernate.html), mas [or mapping](OR%20Mapping.html) es prezentacios frameworkok), a J2EE pedig megmaradt mint kozos alapszolgaltatas.

Gyakorlatilag ez az oldalkomplexum a Enterprise Java-val foglalkozik. Behatarolni nem igazan lehet, mivel gyakorlatilag a programozas minden agat magaba foglalja. Talan azt lehetne mondani, hogy olyan programozasi feladatok megoldasara szolgal az architektura, amik adatbazisintenzivek, skalazhatoak es nagy foku megbizhatosaggal rendelkeznek. De ennel tobbet ne kivanjon tolem senki.

# Arhitektura

Ha jol gondolom, bar ezt leirva sohasem lattam, akkor a J2EE ugy epul fel, hogy az embernek van egy alkalmazas szervere, aztan abba az alkalmazas szerverbe berakja a maga kis produktumat es onnantol kezdve mindenfele nyalanksaghoz hozza tud ferni.

A bizonytalansagom abbol ered, hogy a J2EE API egyes reszei kulon is hasznalhatoak, mig masok csak az alkamazas szerverel egyutt. De hogy melyek ezek? passz:-) Az biztos, hogy az EJB, Servlet+JSP, JMS technologiak csak szerver kontaineren belul hasznalhatoak.

# Reszek

Vegignezve a J2EE API-t, a kovetkezoket latom:

*   [javamail](Missing.html) API: mint a neve is mutatja, level kuldessel foglalkozo API
*   [EJB](EJB.html): Egy masik varazsszo, ami elegge megosztja a Java tarsasagot.
*   Deploy: J2EE Application Deployment. Ez csak az 1.4-es api-tol. A JSR alapjan a kovetkezokkel foglalkozik: Install / Deploy, Config, Undeploy (Eletemben nem lattam)
*   [JNDI](JNDI.html)
*   [JMS](JMS.html): Java Messaging Services. Egy megoldas fuggetlen uzenetkuldo rendszer. Csak annyit mond, hogy hogyan kell / lehet uzeneteket kuldeni kulonbozo resztvevok kozott.
*   [JMX](JMX.html) J2EE Managment
*   Resource ([JCA](JCA.html))
*   [Servlet_jsp](servlet_jsp.html)
*   [XML](XML.html) kezeles
*   [JAXR](JAXR.html)
*   [JTA](JTA.html)
*   [JAX-RPC](JAX-RPC.html)
*   [SOAP](SOAP.html)
*   [XML](XML.html) Transform ([xslt](XSLT.html))

Na most ezekrol azt kell tudni, hogy altalaban nem szolgaltatnak konkret implementaciot, sokkal inkabb interface-eket. Ennek okan, annak ellenere hogy jol meghatarozott dolgokrol van szo, sokszor a kulonbozo alkalmazas szerverek eleg egyedi viselkedeseket tudnak produkalni.

# Linkek

*   Elso es legalapvetobb (Sok, de megeri magad vegigragni rajta...): [http://java.sun.com/j2ee/1.4/docs/tutorial/doc/index.html](http://java.sun.com/j2ee/1.4/docs/tutorial/doc/index.html)

Lasd meg:

*   [alkalmazas szerver](Alkalmazas%20Szerver.html)ek

Folyt. Kov
