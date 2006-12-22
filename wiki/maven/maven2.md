---
creationDate        : 2006-02-08 23:34:14 +0100 
author              : kocka 
title               : maven/maven2 
name                : maven/maven2 
layout              : wiki 
path                : maven/maven2 
date                : 2006-12-22 13:27:19 +0100 
version             : 27 
creator             : kocka 
---

-   [maven/maven2/Archetype](../maven/maven2/Archetype.html)
-   [maven/maven2/mojo](../maven/maven2/mojo.html)
-   [maven/maven2/IDE support](../maven/maven2/IDE support.html)
-   [maven/maven2](../maven/maven2.html)



A maven 1 utan egy nagy refactor kovetkezett, nagytakaritas a pom formatumaban valtozasok, ilyesmi. Ha a [maven/maven1](../maven/maven1.html)gyel problemaid voltak de meg nyitott vagy uj dolgokra, probald ki batran a maven2-t, lenyegesen sokat javit az egyebkent is jo elkepzeles megvalositasan.

*   regi maven peldaul egy pluginen keresztul tamogatta a multiprojecteket, ezt a maven 2 alapbol tudja
*   Minden plugin lett, azaz mindener a halozathoz nyul, az alap cucc csak 1 mega, minden mast csak akkor tolt le ha kell.
*   Uj, a regivel termeszetesen inkompatibilis plugin struktura ([maven/maven2/mojo](../maven/maven2/mojo.html))
*   uj repository struktura (de tamogatja a regit is "legacy" neven)
*   archetype-ok új projectek villám gyors létrehozására ([lista](http://docs.codehaus.org/display/MAVENUSER/Archetypes+List))
*   mirrorozhato a repository, nem al meg az elet ha lehal egy szerver: [http://maven.apache.org/guides/mini/guide-mirror-settings.html](http://maven.apache.org/guides/mini/guide-mirror-settings.html)
*   van hozza proxy szoftver is [http://maven-proxy.codehaus.org/](http://maven-proxy.codehaus.org/) (vagy a [proximity](../proximity.html))
*   build lifecycle koncepcio

[Test](../test.html) frameworkbol tamogatja a [junit](../junit.html) 3.8-at es a [testNG](../testng.html)-t, [junit](../junit.html) 4-el is meg lehet hajtani eppen, ha pont ugyanugy nevezed az metodusokat ahogy 3.8 alatt. [Test/Categorization](../Test/Categorization.html) [junit](../junit.html) 4-hez nincsen sajnos, pedig de jo is lenne, [testng](../testng.html)vel megy siman.

Cikkek:

*   [Get the most out of Maven 2 site generation](http://www.javaworld.com/javaworld/jw-02-2006/jw-0227-maven_p.html)
*   [Maven 2.0: Compile, Test, Run, Deploy, and More](http://www.onjava.com/lpt/a/6528)
*   [The Maven 2 POM demystified](http://www.javaworld.com/javaworld/jw-05-2006/jw-0529-maven.html)

linkek:

*   [http://mvnrepository.com/](http://mvnrepository.com/) (ha valamilyen artifactot keresel, hasznos)
*   [ Maven 2.1 Design Documents](http://docs.codehaus.org/display/MAVEN/Maven+2.1+Design+Documents)

__konyv__:

*   Egy regisztracio utan [letoltheto konyv](http://www.mergere.com/m2book_download.jsp). Beleolvasva: nem rossz. Sajno kuldik a promo leveleket, de a spamfilter hamar megtanulja, meg udvariasak es le is lehet iratkozni :)

__extra repo-k__:

*   [https://maven-repository.dev.java.net/nonav/repository/](https://maven-repository.dev.java.net/nonav/repository/) [leiras](https://maven-repository.dev.java.net/nonav/)
*   central: [http://repo1.maven.org/m2/](http://repo1.maven.org/m2/)
*   [codehaus](../codehaus.html) [http://dist.codehaus.org/](http://dist.codehaus.org/)

__[IDE](../IDE.html) support:__

*   Egy egesz jol fejlodo [eclipse](../Eclipse.html) [eclipse/plug-in](../Eclipse/Plug-in.html) hozza:[http://m2eclipse.codehaus.org/](http://m2eclipse.codehaus.org/)
*   A [mevenide](../mevenide.html) [netbeans](../Netbeans.html) pluginje kivalloan tamogatja, nagyon elegedett voltam vele. Barcsak az [eclipse](../Eclipse.html)-s lenne ilyen franko.
*   Egyebkent ha nem akarsz uj plugint az [ide](../IDE.html)-be akkor mvn eclipse:eclipse annelkul is legeneralja a project descriptorokat, vagy netbeanshoz is van ilyen parancs csak nem tartom fejben :)

__Maven 2 felhasznalok:__

*   [jetty](../jetty.html)
*   [acegi](../acegi.html)
*   [cocoon](../cocoon.html)
*   [spring](../spring.html)? (http://www.bearaway.org/wp/?p=518)
*   es sok mas top project

__Erdekesebb kulso pluginek:__

*   [qalab](../qalab.html)
*   [cargo](../cargo.html)
*   [mavenium](../mavenium.html)

Lasd: [maven](../maven.html), [maven/maven1](../maven/maven1.html), [build](../build.html), [proximity](../proximity.html)


