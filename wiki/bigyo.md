---
creationDate        : 2004-11-24 23:43:17 +0100 
author              : renszarv 
title               : Nevezhetném __MégEgyÚjabbKomponensKeretrendszernek__ de a __bigyo__ rövidebbnek tünt.  
name                : bigyo 
layout              : wiki 
path                : bigyo 
date                : 2004-11-29 22:50:28 +0100 
version             : 3 
creator             : renszarv 
---
 Miért is irtam? 

1.   mert ráértem...
1.   miért ne?
1.   azért mert nem találtam olyan IoC frameworkot ami az igényeimet kielégitette volna. (S itt most szigoruan programozás beli igényeimre gondolok) <br/>

 Nevezetesen:

1.   komponensek közötti függőségek kezelése, s minél transzparensebb felinicalizálása. Mondjuk set-terekkel.
1.   a rendszer intelligensen kezelje a komponens konfigurációját, olyan szinten, hogy ha a VM-ben a komponens megváltoztat valami paramétert, akkor transzparens módon ez megjelenjen a fájl rendszerben. Valamint a másik irányban, ha az ember módositja futás közben a konfig fájlt, akkor erről a komponens értesüljön, s tudjon rá érdemben reagálni. 
1.   Az előzőböl következik, hogy mind emberi mind gépi "kézzel" fájdalom nélkül lehessen szerkeszteni.
1.   JMX-el is lehessen konfigurálni. 

Igazából a 2-es funkciót hiányzott nagyon, de nem láttam sehol sem.
 Úgyhogy végig gondoltam, hogy hogyan szeretnék komponenseket programozni:

*   a perzisztens konfiguráció élesen válljon el a többitől, a konfiguráció legyen egy POJO. Alapvetően nehézkes ötletnek tartom az [avalon](avalon.html)-os [Configuration](Missing.html) interface-ét) Engem nem (nagyon) érdekel, hogy van letárolva. Pláne amikor "büzlik" az olyan jellegü conf.getChild("widget").getAttribute("name"), hogy itt bizony a fejlesztők (namespace-es) XML-en kivül mást el se nagyon birtak képzelni.
*   A konfiguráció legyen egyszerü, és tipusos (tetszőleges tipusokkal természetesen!). A myConfig.getServerName() mondjuk adjon vissza egy String-et, a myConfig.getFile() meg egy File objektumot, esetleg a myConfig.getMiscMap() meg egy Map-et. 
*   Ne a komponens programozójának kelljen bonyolult módon egy DOM-ból kibányászni az információkat.
*   a más komponensen való függőségeket a komponensem kapja meg set-terrel. De ha kell akkor tetszőleges komponenst meg tudjon szerezni (lásd: avalon ServiceManager).
*   ha lehet ne kelljen semmilyen interfacet implementálni a komponensnek. Sőt, a komponensek akkor is müködhessenek, ha nincs a közelben a container. (lásd JUnit tesztelhetőség - mer anélkül nem élünk :) )

Valamint telepítéskor: 

*   Lehessen megadni, hogy melyik komponens "startup" melyiket csak akkor jöjjön létre, ha szükség van rá.
*   Minimális - parancssori - változtatásokkal lehessen módositani, hogy milyen komponens halmazok - azaz profile-ok - legyenek aktivak.  Pl __./runserver \-\-profile=webserver \-\-profile=jmx__ esetén inditsa el azokat a komponenseket amik a "webserver" illetve a "jmx" szolgáltatáshoz szükségesek. 

Nos, ezeket a célokat már a bigyo tudja.

Ráadásul elérhető a [http://bigyo.sourceforge.net](http://bigyo.sourceforge.net) cimen :)


Ha bárki bármit értett belőle, akkor szóljon :)

# [avalon](avalon.html) komponensek [bigyo](bigyo.html) komponensekké alakítása.

A két rendszer nem ugyanazokat a szolgáltatásokat nyújtja a komponenseinek ezért a portolás se nem teljesen zökkenőmentes, se nem teljesen gépiesíthető. 

# Avalon interfacek megfeleltetései:


*   LogEnabled/Logger : 

   Log4j eddig bőven elég volt minden eddigi loggolási igényemhez, nem akartam feltalálni újra a spanyol viaszt. Ha mégis ilyen stilusu loggolást akarnánk használni akkor a következőt kell tennünk:
```
 /**
  * A metodus nev tetszoleges lehet.... 
  * @bigyo-depend logger
  */
  public void setSajatLogger(Logger log) {
```

S majd a példány konfigurációjában meg kell adnunk, hogy melyik - szintén általunk felkonfigurált - Logger példányt szeretnénk használni.

*   Context : ahogy látom ez teljes egészében megfelel a bigyo tipusos konfiguráció fogalmával. Ezután a :

```
  File file = (File)context.get("myFile");
```
 helyett a 
```
  File file = config.getMyFile();
```
 kell hivni. Most mondja valaki, hogy nem egyszerübb :)

*   Configuration/Parameters : szintén az egyszerübb, s testre szabhatóbb saját konfigurációs beanunket használhatjuk.
*   Servicable/ServiceManager : egyrészt a setterekkel definiált serviceket megkapjuk automatikusan a bigyo-tól (ahogy a Logger-nél is irtam) másrészt ha ennél dinamikusabban szeretnénk meg kapni a komponenseinket, akkor 

```
 /**
* @bigyo-depend bigyo:service-locator
*/
public setServiceLocator(net.sf.bigyo.api.ServiceLocator locator)
``` 
 metodus deklarálásával, s a locator segitségével magunkhoz ragadhatunk tetszőleges komponenst. Jelenleg nem lehet release-elni egy komponenst, ha már megszereztük.

*   Lifecycle interface-k: az egész le van egyszerüsitve. Egy komponens megadhat egy start és egy stop metódust (a @bigyo-start és @bigyo-stop tag-gel) s azok a megfelelő időpontban meg lesznek hivva. Még annyi különbség van az avalon lifecycle-hoz képest - s ez különösen az indulásnál látszik - hogy a bigyo elinditáskor elöször létrehozza az összes komponenst, meg hivja a megfelelő set-ter metódusokat, aztán amikor minden példány létezik utánna egy menetben hivja végig az összes start metódust.
