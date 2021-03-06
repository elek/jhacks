---
creationDate        : 2004-07-26 17:23:25 +0200 
author              : karenin 
title               : maven 
name                : maven 
layout              : wiki 
path                : maven 
date                : 2008-07-23 07:19:26 +0200 
version             : 27 
creator             : kocka 
---
![image](http://maven.apache.org/images/maven-small.gif)(http://maven.apache.org)<br/>
[irc://irc.codehaus.org/maven](irc://irc.codehaus.org/maven)


-   [maven](maven.html)
-   [mavenium](mavenium.html)
-   [maven/maven2/Archetype](maven/maven2/Archetype.html)
-   [maven/maven2/mojo](maven/maven2/mojo.html)
-   [maven/maven2/IDE support](maven/maven2/IDE support.html)
-   [maven/maven2](maven/maven2.html)
-   [maven/maven1](maven/maven1.html)



Egy java [build](build.html) tool, erosen epit az [ant](ant.html)ra, uj reteget kepez felette. Ket, egymastol eleg erosen kulonbozo verzioja van: [maven/maven1](maven/maven1.html) es [maven/maven2](maven/maven2.html) Gyorsan osszehasonlitva az plain [ant](ant.html)-tal:

1.   __legfontosabb kulonbseg:__ a maven fejlesztesi processz, nem csak [build](build.html) tool
1.   Sok __elore megirt goal__-t tartalmaz, igy a fejlesztoknek mar csak ritkan kell sajatot irniuk, ez kb az ant targetnek felel meg, de ilyet csak specialis esetekben kell irni
1.   __kozponti repository__ a fuggosegek tarolasara. Alapbol ez a [http://www.ibiblio.irg/maven](http://www.ibiblio.irg/maven) Minden dependency innen toltodik le a local cache-be (kellemetlen amikor gprs-ed van, akkor meg foleg amikor leall az ibiblio szerver)
1.   A __POM__ (project object model) tartalmazza a legfontosabb informaciokat a projectedrol, es azokat a pluginok fel is hasznalhatjak. Altalanos informaciok, mint bugtrackered url-je, cvs vagy svn hozzaferes, levlistak, satobbi. Ami nem fer bele a POM-ba, mert pl plugin fuggo, azt a project.properties-ban definialhatod tulajdonsagkent.
1.   Ant taskdef helyett pluginek. A pluginek is termeszetesen a kozponti repo-bol jonnek. Persze hasznalhatod az ant taskokat is.


Ha meg akarod szeretni a maven-t probald ki a weboldal generalast \(maven site\) vagy a distribution generaciot \(maven dist\), probald ki a [mevenide](mevenide.html)-t is [eclipse](Eclipse.html)hez vagy [netbeans](Netbeans.html)hoz: [http://mevenide.codehaus.org/](http://mevenide.codehaus.org/)

A szopas a maven-ben:

1.   [maven/maven1](maven/maven1.html): amikor az arcodba vagja az erthetetlen [jelly](jelly.html) stacktraceit (hala jehovanak most mar azert ritkan)
1.   amikor nincs neted (de az amugy is)
1.   van amikor egyszeruen proceduralisan leirni a build menetet egyszerubb (ilyenkor jon az [ant](ant.html)) (bar szerintem ez ritkabb)
1.   [maven/maven1](maven/maven1.html): amikor sokszor kell buildelned, s nincs kedved 20 másodperceket várni, hogy elinduljon, amikor csak egy forditás és jar-olás lenne a feladat. Hala jehovanak a [maven/maven2](maven/maven2.html) tenyleg sokkal gyorsabb, meg kissebb is (ugy 1 mega).


linkek:

*   Maven: The Definitive guide: [http://www.sonatype.com/book/](http://www.sonatype.com/book/) Ha részletes leírásra vágysz, az egyik legjobb.
*   egy kis osszefoglalo es migracio howto: [http://www.onjava.com/lpt/a/5048](http://www.onjava.com/lpt/a/5048)
*   maven bugok :) [http://jira.codehaus.org/](http://jira.codehaus.org/)
*   aki szereti a papirt: [http://www.oreilly.com/catalog/mavenadn/index.html](http://www.oreilly.com/catalog/mavenadn/index.html) [http://www.mavenbook.org/](http://www.mavenbook.org/) (csak a forraskodok a konyvhoz)
*   [j2ee](j2ee.html) with maven: [Building J2EE Projects with Maven](http://www.onjava.com/pub/a/onjava/2005/09/07/maven.html)

Lasd meg: [build](build.html), [continuum](continuum.html)


