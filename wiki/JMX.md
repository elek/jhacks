---
creationDate        : 2004-08-06 11:00:24 +0200 
author              : admin 
title               : JMX 
name                : JMX 
layout              : wiki 
path                : JMX 
date                : 2006-03-26 01:42:43 +0100 
version             : 1 
creator             : kocka 
---
__Java Management Extenxion__

JMX alapgondolata: adsz egy MBean-t, ami tudja hogy a komponensedet hogyan lehet managelni, a container pedig ad egyreszt JMX kornyezetet, masreszt JMX adaptereket. Ilyen lehet PL egy http vagy egy [RMI](RMI.html) adapter, aztan kulonbozo felhasznaloi feluletet is adhatsz ra. Igy elvalasztottuk egymastol a komponenst a komponens managementjet, es a management felhasznalo feluletet.

Itt erdemes megemliteni az [IOC](ioc.html) rendszereket, mert szerintem egy szerver oldali [IOC](ioc.html)-ben fontos hogy legyen JMX, valamint a [J2EE](j2ee.html) rendszereknek is szabvanyos resze.

Nagy kedvencem a [loom](loom.html) JMX adaptere.
