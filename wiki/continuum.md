---
creationDate        : 2005-04-27 09:54:13 +0200 
author              : kocka 
title               : continuum 
name                : continuum 
layout              : wiki 
path                : continuum 
date                : 2006-04-17 09:55:58 +0200 
version             : 12 
creator             : kocka 
---
![image](http://maven.apache.org/continuum/images/continuum_logo_75.gif)(http://maven.apache.org/continuum/)

Egy [Continuous Integration](Continuous%20Integration.html) tool, az [asf](ASF.html) fejleszteseben. A Continuum leginkab a [maven](maven.html) fejlesztoket szolgalja ki, de tamogatja az [ant](ant.html) projecteket is, meg ha nagyon kell akkor a shelles megoldassal a [C](C.html) meg make-os projecteket is lefordithatod, de arra vegulis egy cron job is jo :-D

Egyebkent [plexus](plexus.html) [ioc](ioc.html) kontenerben fut es [jetty](jetty.html) beagyazasaval egy [webapp](webapp.html) feluleten hasznalhatod, valamint backendkent hasznalhatsz tulajdonkeppen barmilyen [RDBMS](RDBMS.html)t, defaultbol ez [derby](Derby.html), igazabol ilyen kis adatbazishoz siman eleg is. A [plexus](plexus.html)nak koszonhetoen pedig  elmeletileg keves munkaval megoldhato hogy mas szoftvereket is futtathass ugyanabban a Vmben, ha meg kell huzni a derekszijat.

Amivel erdemesse valik nagyobb ceges felhasznalasra is, az a felhasznalo es csoportkezelese, kioszthato hogy melyik csoport tid projecteket felvenni, buildeket inditani, stb. Na meg persze minden projecthez rendelhetsz kulon notifyereket: [irc](irc.html), [msn](Missing.html), [mail](mail.html), [jabber](jabber.html) amellett hogy a webes interface-n keresztul is hozzaferhetsz a logokhoz.

Van, pontosabban lenne neki egy szep [xfire](xfire.html)-os web services interface is, ez viszont teljesen eltort es alapbol ki van belole iktatva. Szoval nincs, de lehetne :)

[maven2](Missing.html) projectek eseteben igazan sokmindennel kapraztatja el a felhasznalot, peldaul a pom-bol kiszedi hogy kinek kell szolnia buildeles eseten, kulon projectkent jegyzi be a modulokat.

Szivasok:

*   ha egy sourceforge-os svn repot akarsz hasznalni, de meg nem trustoltad a sourceforge svn repo kulcsat, ilyenkor addig anyaz amig svn klienssel ki nem csekoutolsz egy tetszoleges projectet es el nem fogadod orokre a kulcsot
