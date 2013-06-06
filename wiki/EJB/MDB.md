---
creationDate        : 2005-10-19 22:50:26 +0200 
author              : kocka 
title               : Message Driven Bean 
name                : EJB/MDB 
layout              : wiki 
path                : EJB/MDB 
date                : 2007-01-31 21:02:52 +0100 
version             : 2 
creator             : kocka 
---
Az [EJB](../EJB.html) szabvany altal definialt bean tipus, amit a rendszer fog meghivni egy [JMS](../JMS.html) message erkezesekor.

Olyan dolgokra lett kitalalva, hogy a nagy muveletigenyu/hosszu folyamatokat asszinkron vegezhesd el. pl juzer regisztracio eseteben ellenorzes valami kulso rendszeren, levelkikuldes, stb, mindezt egy sajat kulon tranzakcioban.

Egy erdekes, portolhatobb [pojo](../pojo.html) alternativa a [jnecks](../JNecks.html).
