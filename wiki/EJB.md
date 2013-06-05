---
creationDate: 1090942127037 
author: karenin 
contentAuthor: karenin 
title: EJB 
contentUpdateDate: 1223364627171 
name: EJB 
layout: wiki 
date: 1223364627171 
creator: zsoltk 
---


# A varazsszo.

Mielőtt elrettennél a használatától: A következő bekezdések jórészt az EJB2-re vonatkoznak. Azóta megjelent az [EJB3](EJB3.html), ami visszafelé kompatibilis az EJB2-vel és jóval kényelmesebb a használata. A [J2EE](j2ee.html) (manapság Java EE) specifikáció gyüjtemény egy reprezentás tagja).

Tulajdonképpen egy alkalmazásfejlesztő keretrendszer, tipikusan az üzleti logika implementására. Ahogy neve is mutatja Bean-ek családjáról szól. Ezek lehetnek:

## Session beanek

Ezekbe kerül az üzleti logika. Lehet Stateless és Statefull. Az utóbbit őgy képzeljük el, mintha a metódusok hívása között nálunk maradna egy Session, és az alapján valamifajta állapotot kapcsolna hozzánk a Bean. Alaphelyzetben a Session beanek kezelik a tranzakviókat (jó sok fajta beállítás van, hogy ha épp nincs tranzakció mit csináljon, és ha van akkor mit), vannak benne mindenféle interceptorok (létrehozás előtt, után meghívandó életciklus függvények), tud időzítést, és persze a beaneknek van állapota is, mivel poolozódnak és ide oda mentegetődnek a rendszerben. (És mindezt szemrebbenés nélkül csinálja clusterezett környezetben is.)

## [Entity beanek](EJB/entity%20bean.html)

Vagy entitások. Ez [EJB3](EJB3.html) óta [JPA](JPA.html) néven fut, előtte egy kissé bonyoldalmas megoldás volt rá, ne akard tudni, hogy hogy nézett ki. EJB3-ba igazából már sima [POJO](pojo.html)-k, amik egy [ORM](ORM.html) mapping részei.

## [Message Driven Beanek](EJB/MDB.html)

Ezek aszinkron üzenetek feldolgozására valók (tipikusan JMS).

Az egész szoksásoan becsomagolható valami szabály szeirnt, és deployolható.

# Verziók

Jelenleg az EJB 3.1 van fejlesztés alatt, és az EJB 3 a stabil verzió. Az EJB 2, 2.1-et már csak nagyon legacy rendszerekbe használják. Ez a régi változat, még elég bonyolult volt, mindenféle interfacekkel kellet trükközni, és API-t leszármaztatni, és ezt az egészet még némi bonyolult XML leíró is fűszerezte. Az EJB 3-ra leegyszerűsödött, ahol is a modern trendeknek megfelelően mindenhol POJO-t lehet használni, amit aztán oda vissza lehet annotálni. Szóval használható lett. 

Az viszont fontos, hogy az EJB 2.1-nél a háttérben ugyanaz megy, mint az EJB3-nál, csak a használat lett egyszerűbb, tehát a régi tudás teljesen használható.

Ha a régi EJB érdekel, nézd meg az [eredeti](EJB2.html) wiki oldalt, ami akkor készült, amikor még EJB3 nem volt.

A következő verzió az EJB 3.1 lesz, ami várhatóan a 2009-es [JavaOne](JavaOne.html)-ra készül el. (Public Review már van). Jobban fog hasonlítani egy IoC konténerre, futni fog [Java SE](Missing.html)-ben is, lesz Lite profilja is, a Timer részeket is végre megcsinálják, stb.

EJB 3:

*   http://today.java.net/pub/a/today/2004/08/05/ejbnewlife.html



Erdekessegek:
*   http://www.javaworld.com/javaworld/jw-12-2000/jw-1215-anyclass.html



Site-ok:
*   http://www.ejbsig.de/



Lasd meg: [JNDI](JNDI.html), [persistence](persistence.html), [JDBC](JDBC.html), [J2EE](j2ee.html), [RDBMS](RDBMS.html), [IDE](IDE.html)




