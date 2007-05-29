---
creationDate        : 2007-05-29 16:10:01 +0200 
author              : kocka 
title               : struts/struts 1 
name                : struts/struts 1 
layout              : wiki 
path                : struts/struts 1 
date                : 2007-05-29 16:58:38 +0200 
version             : 5 
creator             : kocka 
---
![image](http://struts.apache.org/images/struts.gif)(http://jakarta.apache.org/struts/)

(strucc, [hunglish](../hunglish.html)ban igy ejtjuk)


A hatranya az irdatlan nagyra novo xml fileok, meg az hogy ha nincs tool-od akkor kezzel kell :( Muszaj valami tool-t hasznalni:

*   [Websphere App Dev](../Websphere%20App%20Dev.html) (kivallo struts support, sajnos eleg dragan)
*   [Oracle](../Oracle.html) [JDeveloper](../JDeveloper.html)-ben is tudsz struccos alkalmazast csinalni, hasonlo modon mint AppDev-ben.
*   [myeclipse](../myeclipse.html) szinten pezert ([linux 48](../Linux%2048.html)on stabilnak bizonyult)
*   [StrutsBox](../StrutsBox.html) ingyen de kicsit furi dolog
*   [vim](../VIM.html) yeah!!! :-D


hasznos, OSS eszkoz lehet a [xdoclet](../XDoclet.html), mint a legtob esetben :)

*   __struts-module__: egy struts konfiguracios file, es az altala tartalmazott alkalmazas objektumok. (nyilvan lehet tobb is)
*   __formbean__: olyan bean, ami a formodrol szarmazo adatokat tartalmazza. ket jelentosege van: 1, nem neked kell szaroznod az adatok parselesevel, 2, az actionod vegre bean-t kap, nem egy request objektumot. Opcionalisan implementalhatod a validate metodust, amivel a nem evidens hibakat detektalhatod (pl amikor az e-mail cim nem e-mail cim, vagy a jelszo mezo ures, ilyesmi)
*   __action__: egy osztaly ami a [http](../HTTP.html) actionodat reprezentalja. Az action formbean-t kap, es ha nem dob egy exceptiont-t, akkor actionforwardot ad vissza. Az actionforward mondja meg hogy melyik [jsp](../JSP.html) adja majd a kimenetet. Fontos megemliteni hogy az Action threadsafe kell hogy legyen mert csak egy peldanyosul belole.
*   __exception__: a hetkoznapi exception, annyi extraval, hogy a struts modulban definialhatod hogy melyik [jsp](../JSP.html)-t kell megjelenitani ha a vezerlo [servlet](../servlet.html) azt kapja az actionodtol.
*   __i18n__: a struts nagyon tamogatja az [i18n](../i18n.html)-t, minden felhasznalo szamara megjelenitett szoveget az alkalmazas eroforrasokbol keres ki.
*   __tagek__: a struts jonehany taggel neheziti meg a [jsp](../JSP.html) fejlesztok eletet, koztuk [i18n](../i18n.html), bean kezeles, meg ilyesmi...
*   __tiles__: Ez a view komponenesek ujrafelhasznalhatosagara szolgal, sajna ahany struts verzio megjelent eddig, annyifelekeppen mukodik benne, ami meglehetosen megneheziti hasznalatat. Termeszetesen nincs a jelenlegi verziorol dokumentacio :-D

Lasd meg:  [beehive](../beehive.html), [webapp](../webapp.html), [mvc](../MVC.html)

Cikkek: 

*   [Get a better handle on Struts actions, with Spring](http://www-128.ibm.com/developerworks/java/library/j-sr2.html)

Rokonsagok mas rendszerekkel:

*   Integracio a [Spring](../spring.html)gel, ez ugy nez ki hogy a springes applicationcontext-et elkerheted a megfelelo osztalybol leszarmaztatott actionokbol. Szoval nem tul barati. A masik lehetoseg az hogy a spring maga jegyzi be az actionokat, es settereken keresztul be tudod pakolgatni a dependencyket. Szoval ez mar szeretnivalobb, viszont az meg nem tiszta hogy a [tiles](../tiles.html) controllereket hogyan lehet vele kezelni, ha lehet egyaltalan... mert annelkul loszart nem er az egesz. Erre amugy csinaltam egy osztalyt ami lehetove teszi hogy a Controller benajeidet a [spring](../spring.html) alkalmazas kontextusba pakold, de meg en se szeretem :)
*   [webwork](../WebWork.html)
*   [jsf](../JSF.html)


