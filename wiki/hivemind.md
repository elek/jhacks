---
creationDate        : 2004-08-06 23:04:14 +0200 
author              : admin 
title               : hivemind 
name                : hivemind 
layout              : wiki 
path                : hivemind 
date                : 2006-03-26 01:48:01 +0100 
version             : 1 
creator             : stoned 
---
Az [IoC](ioc.html)/[Dependency injection](dependency%20injection.html)/[SOA](SOA.html) konténerek egyre népesebb táborának tagja. Fejlesztését az a Howard Lewis Ship kezdte, akinek a nagyszerű [Tapestry](tapestry.html) frameworköt köszönhetjük (a Tapestry 3.1 a hivemind-ra fog épülni).

Első blikkre a hivemind csak egy az egyre szaporodó konténerek közül, de ha az ember jobban belenéz ezek világába, látszik, hogy egy-egy konténer főbb céljai eltérnek egymástól. Mint minden igazán jó project, ez is speciális szükségeletek kielégítésére jött létre, és később fejlődött azzá, ami. A [Avalon](avalon.html) ugye a JServ ([Tomcat](tomcat.html) előd) project [design pattern](Missing.html)-jeit hasznosítja, a [spring](spring.html)et az [EJB](EJB.html) által keltett frusztráció szülte a világra, a hivemind... nos a hivemind azért jött létre, mert egy EJB alkalmazásban összegyűlt néhány tucatnyi task, amit az alkalmazás indulásakor végre kellett hajtani. Ehhez egy BEA specifikus hookot és egy Stateless Session Bean-t használtak, ahol erősen kellett figyelni a taskok sorrendjére, elkezdett hízni a bean, emellett a függőségei kiterjedtek a teljes alkalmazásra.

Ezután a kis félrevezető bevezető után talán térjünk rá a lényegre. Hivemind alapvető fogalmak:

*   __Services__ : Míg a [spring](spring.html)-ben beanekről beszélünk, a hivemindban ezeket service-eknek hívjuk. Ez nem csak elnevezési különbség, ugyanis a springben bármilyen bean (ehh, buzzword ez is, bármilyen objektum) létrehozható, a hivemindban egy service nem több, mint __egy__ interface. Legalábbis az alkalmazás többi részének. Természetesen ezen service-ek implementációja hagyományos objektum (azaz [POJO](pojo.html)), amik függnek a többi szervíztől, és még konfigurálni is kell őket.
*   __Configuration__ : Ez szinte egy framework a frameworkben. A konfiguráció formátumát a fejlesztő határozhatja meg. Ami nem egészen igaz, mert annyi kikötés van, hogy XML formátumnak kell lennie, és a module descriptorban kell megadni. Ha ez egy kicsit homályos, akkor az az én hibám :-). A lényeg az, hogy a fejlesztő meghatároz egy konfigurációs sémát, ami egy szabálygyűjtemény, ami meghatározza a konfiguráció megadásának módját (~XML séma). A séma a megadott konfigurációs adatból egy vagy több objektumot állít elő. A service már ezeket az objektumokat kapja meg, mint konfiguráció. Ez némi előrelépés az avalonban látható Configuration.getChild() plumbinghoz képest. Asszem :-) (ja, és ez sokkal egyszerűbb, mint aminek elsőre tűnik).
*   __Microkernel__ : Az egészet egy microkernel fogja össze, ami gondoskodik a service-ek megfelelő időben történő létrehozásáról (lazy v. eager initialization), konfigurálásáról, a függőségek összekapcsolásáról, némi AOP szerű funkcionalitással vegyítve (csak interceptorok). Mindezt a module deployment descriptorok parse-olása után.

A végeredmény az, hogy az alkalmazás kódja mentes mindenféle framework függőségtől (bár lehetőség van egy lifecycle interface implementálására, ami nem javallot általában). A függőségek mint interface-ek, a konfiguráció mint objektumok jelennek meg a kódban.

Nos, eddig semmi különös, igaz? Azért van még miről mesélni :-). Az egyik érdekes dolog a modulok. Tegyük fel, hogy Kis Béla programozó fejleszti a cég security frameworkjét, amit majd több alkalmazásban akarnak felhsználni. Első dolga, hogy kialakítson egy API-t (az egyszerűség kedvéért tegyük fel, hogy így csinálja :-)), ami pár interface-t jelent. Ezeket az interface-eket, a hozzájuk tartozó support classokkal, exceptionökkel, stb. becsomagolja egy .jar archívba egy module descriptor társaságában. Ez a modul descriptor meghatároz legelőször egy namespace-t(com.acme.security), minden service-hez (pl. AuthenticationService) egy __service-pointot__, egy-két __konfigurációs sémát__.

Ezután implementálja az adott interfészeket, teszteli a kódot (POJO-k, egyszerű tesztelni), majd ezt az implementációt egy másik .jar file-ba csomagolja, egy másik module-descriptor társaságában. Ez a module descriptor (namespace: com.acme.security.ldap) hozzáadja az implementációkat az előző modulban deklarált service-pointokhoz. Az implementációt az előző modulban meghatározott séma alapján konfigurálja.

Király! Van egy API-nk és egy implementációnk. Most akkor mi? Egyszerű. A két .jar-t be kell passzintani az alkalmazásunk classpath-jába, és...
```
Registry registry = RegistryBuilder.constructDefaultRegistry();
AuthenticationService authService = 
  (AuthenticationService) registry.getService(AuthenticationService.class);
// vagy explicit megadva a full q. service nevet
AuthenticationService authService = 
  (AuthenticationService) registry.getService(
    "com.acme.security.AuthenticationService",
    AuthenticationService.class);

```

Ha másik implementációt akarunk, csak kicseréljük az implementációt tartalmazó .jar-t egy másikra. Ha véletlenül két implementációnk lenne, vagy egy sem, a registry attól még felépül (by default), logolva a hiányzó/duplicate service-eket (lehetőség van konfigurálni, hogy ilyenkor dobjob egy hátast meg egy exception-t).

A registry létrehozását és eltárolását természetesen egyszer kell elvégezni (pl. egy servlet initialize() metódusában, majd a servlet contextben eltárolni a registry-t).

__Service modellek__

*   primitive : Az alap. A framework az első hivatkozáskor példányosítja a service-t
*   singleton : A framework a service implementáció helyett egy proxy-t ad vissza (ami implementálja a service interface-t). Az első metódushívás során a proxy példányosítja a service-t. Ennek akkor van jelentősége, ha a service létrehozása sok költséggel jár.
*   threaded : A variációk ThreadLocalra című sorozat egy újabb része. Minden threadnek saját példánya van a service-ből. Nem kell ecsetelni, hogy ezzel elkerülhető a statikus utility classekbe ágyazott ThreadLocalok. Cool.
*   pooled : Ugyanaz mint a threaded, azzal a különbséggel, hogy minden thread egy poolból kapja a service-t. Ennél és a threaded modelnél szintén proxy magic zajlik a háttérben, nekünk semmivel sem kell törődni. Ja de. Lehetőség van lifecycle interface-ek implementálására (threaded: Discardable, pooled: PoolManageable).

__Service lifecycle__

Mint minden jobb családból származó konténer esetében (és nem minden jobb konténerből származó család esetében) a servicek életciklusa konfigurálható. Minden service (kivéve a threaded, ahol nincs értelme) implementálhatja a RegistryShutdownListener interface-t. Ez egy callback interface, amit a registry hív meg mikor azt lekapcsolják :-). Így a service-ek felsöpörhetik a portájukat a munka végeztével.

Ajánlatos a service-eket singleton modelként létrehozni (ami a default) ha nincs szükségünk a threaded féle modelre, mert a service proxy nem enged újabb hívásokat a registry shutdown után. A primitive service-nél, ahol nem játszik a proxy erre nincs lehetőség.

__Egyéb nyalánkságok__ 

A moduldescriptorokból szép, böngészhető dokumentáció készíthető. Megintcsak: cool.

Spring integráció (SpringLookupFactory). Mivel a hivemindban nincs konyhapult, ezért ez is jól jöhet.

Ha meg is akarod érteni a hivemindot, akkor ajánlom a következő helyet:
[http://jakarta.apache.org/hivemind](http://jakarta.apache.org/hivemind)
Itt mindent megtalálsz, ami kell :-)
