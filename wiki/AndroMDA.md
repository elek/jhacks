---
creationDate: 1092595524096 
author: kocka 
contentAuthor: kocka 
title: AndroMDA 
contentUpdateDate: 1190629693147 
name: AndroMDA 
layout: wiki 
date: 1190629693147 
creator: zsoltk 
---
Az egyik szent tehen, az [MDA](MDA.html) szabadforrasu tamogatoja. Nem titkolt celja, hogy olyan program legyen, ami fogja a jo kis [XMI](Missing.html)-ben leirt diagrammodat es kigeneralja belole a forraskodot. Perpillanat Java-t tamogat.

Az AndroMDA nem kulonallo programkent, hanem egy [Ant](ant.html) taskkent mukodik: fogja a jo kis [XMI](Missing.html) modellt, feldolgozza azt a [Velocity](Velocity.html) segitsegevel, aztan meghivja a sajat belso dolgait, hogy megcsinalja azt, amire kitalaltak.

Perpillanat ezeket tudja:

*   andromda-java: a cartridge that generates general Java source code.
*   andromda-ejb: generates Enterprise JavaBeans.
*   andromda-hibernate: generates persistent classes for the Hibernate O/R mapper.
*   andromda-struts: generates web pages, forms and action classes for use with Jakarta Struts.



link: 
*   http://www.andromda.org
*   [Auth Gábor cikke a javaforum.hu-n](http://www.javaforum.hu/articles/java_forum_20/model_driven_architecture_vagyis_mda/) Most veszem észre hogy ez már [mavennel](maven/maven2.html) megy, kicsit elszált az idő efelett a snipp felett. ([TODO](TODO.html)!!!)
