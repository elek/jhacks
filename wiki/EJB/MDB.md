---
creationDate: 1129755026911 
author: kocka 
contentAuthor: kocka 
title: Message Driven Bean 
contentUpdateDate: 1170273772129 
name: EJBMDB 
layout: wiki 
date: 1170273772129 
creator: kocka 
---
Az [EJB](EJB.html) szabvany altal definialt bean tipus, amit a rendszer fog meghivni egy [JMS](JMS.html) message erkezesekor.

Olyan dolgokra lett kitalalva, hogy a nagy muveletigenyu/hosszu folyamatokat asszinkron vegezhesd el. pl juzer regisztracio eseteben ellenorzes valami kulso rendszeren, levelkikuldes, stb, mindezt egy sajat kulon tranzakcioban.

Egy erdekes, portolhatobb [pojo](pojo.html) alternativa a [jnecks](JNecks.html).
