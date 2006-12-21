---
creationDate        : 2005-02-01 09:16:21 +0100 
author              : kocka 
title               : pojo 
name                : pojo 
layout              : wiki 
path                : pojo 
date                : 2006-12-21 10:27:26 +0100 
version             : 5 
creator             : kocka 
---
__Plain Old Java Object__

Az [IoC](ioc.html) frameworkokkel, [EJB](EJB.html)vel es mas programozasi kornyezetekkel kapcsolatban merult fel az, hogy jopar framework sajat interface-k implementalasat koveteli meg. Igy framework fuggove valik a kod implementacio. Ettol maga a kod ami sok munkaba kerult ugyibar, kontextus fuggove valik, meg mivel tele van ragaszto ('boiler-plate') koddal, ami rontja a karbantarthatosagot.

Ezt kikerulendo, egyszeruen csak "sima oreg [java](java.html) osztalyokkent" (Innen a nev -> __plain old java objects__) implementalsz osztalyokat, aztan vagy wrapeled oket, vagy extendeled sajat osztallyal, igy teszed elfogadhatova a frameorkok szamara, ha egyaltalan szukseg van ilyesmire. (ugyanis nem mindenkinek kellenek lifecycle interfacek)

A [persistence](persistence.html) bean-ekkel kapcsolatban is ugyanez a kerdeskor merult fel, a legtobb fejleszto szereti ha a adatot reprezentalo beanek nem tudnak a sajat tarolasuk modjarol, azaz nem tartalmaznak pl [jdbc](JDBC.html) vagy mas kontextusfuggo kodot.


