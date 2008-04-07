---
creationDate        : 2005-01-30 12:04:29 +0100 
author              : karenin 
title               : OSGi 
name                : OSGi 
layout              : wiki 
path                : OSGi 
date                : 2008-04-08 00:42:31 +0200 
version             : 15 
creator             : kocka 
---
[http://www.osgi.org/](http://www.osgi.org/)

Az egyik legpatinásabb Java alapú [Module System](Module%20System.html). A modulokat Bundle-nek hívja, ami egy Jar file, amiben egy Manifest-ben lehet megmondani, hogy mik azok a szolgáltatások/osztályok, amiket a külső szemlélő használhat belőle, és mik azok, amik csak belső implementációk. A moduluk életciklusa szabályozva van, és futás közben állíthatóak le és indíthatóak újra a modulok. Ezekből már sejteni lehet, hogy egy OSGi framework egyáltalán nem triviális Class Loader-ekből áll, viszont az eredmény nagyon egyszerűen és könnyen használható rendszert adhat. 

Elég széleskörben elterjedt, pl. az [Eclipse](Eclipse.html) is erre épül, de újabban a [Spring](spring.html) alapjaiba is egyre jobban beszivárog.

Mostanában elég durcásak az OSGi hívők, mert a Sun inkább a [JSR-277](JSR-277.html)-et nyomja (ami nem pont ugyanaz, de van elég nagy átfedés). Ezért gyorsan rá is üttettek egy JSR-291-es pecsétet a kész specifikácóra. (lásd még [JCP](jcp.html))

# Implmentációk


*   Knopflerfish [http://www.knopflerfish.org/](http://www.knopflerfish.org/)
*   Equinox, amire az [eclipse](Eclipse.html) is épül, de pl. szerver oldali verziója is van.
*   Felix az [apache](ASF.html) verziója

# Linkek

*   OpenSource implementációk [összehasonlítás](http://www.pierocampanelli.info/articles/2007/01/22/status-of-opensource-osgi-containers)
*   [OSGi, the good the bad the ugly](http://www.parleys.com/display/PARLEYS/OSGi%2C+the+good+the+bad+the+ugly) (prezentacio)
*   [Spring OSGi](http://www.parleys.com/display/PARLEYS/Spring+OSGi) (prezentacio)
*   [Getting Started with OSGi](http://live.eclipse.org/node/407) (prezentációk - [eclipse](Eclipse.html))

# OSGit használó rendszerek

*   [IDE](IDE.html)
    *   [eclipse](Eclipse.html)
*   [alkalmazás szerver](Alkalmazas%20Szerver.html)
    *   [jonas](jonas.html) (5.0-tól)


