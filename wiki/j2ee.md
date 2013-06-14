---
creationDate        : 2004-07-28 14:32:48 +0200 
author              : kocka 
title               : J2EE / JEE 
name                : j2ee 
layout              : wiki 
path                : j2ee 
date                : 2008-06-08 17:23:19 +0200 
version             : 12 
creator             : zsoltk 
---
[![image](http://hackers.forgeahead.hu/space/SnipSnap/config/j2ee_jdk_button_classic_red.gif)](http://java.sun.com/j2ee/download.html)

Java (2) Enterprise Edition.

# Bevezeto

A J2EE a [java](java.html) programozasi nyelv szerveroldali felhasznalasat celzo APIk gyujtemenye, azaz eredetileg fokent olyan dolgok amik ceges felhasznalasra lettek kitalalva. Az idok soran azonban (mikozben a J2EE-bol JavaEE-lett) jol atalakult, ma mar inkabb azt lehetne mondani, hogy minen ami webes Java. A J2EE tervezoi egy tobbretegu hierarchiat almodtak meg, ami az [EJB](EJB.html), [JCA](JCA.html), [servlet](servlet.html), [jsp](JSP.html) reszekbol allt nagyjabol, amit igazabol azt hiszem eleg kevesen vetettek be. Ugyanis eleg sok uj dolgot kellett volna megtanulni, bar ezt szet lehetett volna bontani a [j2ee development roles](j2ee%20development%20roles.html) szerint, de a gyakorlatban azt lattuk hogy valami miatt megsem tortent igy. Igy aztan szuletett mindenfele, a stack bizonyos reszet helyettesito megoldas ([spring](spring.html), [struts](struts.html), [tapestry](tapestry.html), [hibernate](Hibernate.html), mas [or mapping](OR%20Mapping.html) es prezentacios frameworkok), a J2EE pedig megmaradt mint kozos alapszolgaltatas.

A J2EE igazabol az 1.3-as verzioju szabvannyal lett hirhedt, amikoris az EJB programozas jol el volt bonyolitva a konkurens frameworkokhoz kepest, viszont nem nyujtott sokkal tobbet. Az 1.5/1.6 os szabvany azonban nagy hangsulyt fektetett az egyszeru kezelhetosegre, raadasul minden annotacio alapu lett, mindez sokat segitett ahhoz, hogy vegre ne csak az enterprise ceges vilagban terjeden.

# Reszek

Apik:

*   [javamail](Missing.html) API: mint a neve is mutatja, level kuldessel foglalkozo API
*   [EJB](EJB.html): Egy masik varazsszo, ami elegge megosztja a Java tarsasagot.
*   Deploy: J2EE Application Deployment. Ez csak az 1.4-es api-tol. A JSR alapjan a kovetkezokkel foglalkozik: Install / Deploy, Config, Undeploy (Eletemben nem lattam)
*   [JNDI](JNDI.html)
*   [JMS](JMS.html)
*   [JMX](JMX.html) J2EE Managment
*   [JCA](JCA.html)
*   [Servlet_jsp](servlet_jsp.html)
*   [JAXR](JAXR.html)
*   [JTA](JTA.html)
*   [JAX-RPC](JAX-RPC.html)

# Linkek

*   Elso es legalapvetobb (Sok, de megeri magad vegigragni rajta...): [http://java.sun.com/j2ee/1.4/docs/tutorial/doc/index.html](http://java.sun.com/j2ee/1.4/docs/tutorial/doc/index.html)

Lasd meg:

*   [alkalmazas szerver](Alkalmazas%20Szerver.html)ek


