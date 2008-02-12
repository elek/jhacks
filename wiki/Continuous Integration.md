---
creationDate        : 2005-04-27 09:58:41 +0200 
author              : kocka 
title               : Continuous Integration 
name                : Continuous Integration 
layout              : wiki 
path                : Continuous Integration 
date                : 2008-02-12 15:06:27 +0100 
version             : 15 
creator             : kocka 
---
[http://www.martinfowler.com/articles/continuousIntegration.html](http://www.martinfowler.com/articles/continuousIntegration.html)

Nagyon hasznos lehet ha valaki idonkent felhivja a figyelmedet arra hogy valamelyik funkcionalitas a projectben eltorott, foleg ha az illeto nem az ugyfeled ;) es meg csak nem is egy fizetett tesztelo, hanem egy program.

Gyakorlatilag egy eszkoz ami rendszeresen lebuildeli az cuccodat, lefuttatja rajta a teszteket, es ertesit az eredmenyerol. Eleg sok ilyen eszkoz van.

[Open source](Open%20Source.html) es free:

*   [continuum](continuum.html)
*   [damagecontrol](damagecontrol.html)
*   [luntbuild](Missing.html)
*   [gump](gump.html)?
*   [cruisecontrol](cruisecontrol.html)
*   [hudson](https://hudson.dev.java.net/)
*   [sonar](http://sonar.hortis.ch) - olyasmi, nem igazán CI (egyébként talán egy CI szervernek tudnia kellene ilyeneket)

Burzsujoknak:

*   [bamboo](http://www.atlassian.com/software/bamboo/) (atlassian) [Open Source](Open%20Source.html) projectekhez lehet használni, ha publikus lesz az instance
*   [teamcity](http://www.jetbrains.com/teamcity/) (jetbrains) 20 fejlesztő 20 project 20 build definition és így tovább ha nem túl kicsi korlát, akkor a professional ingyen kapható és ugyanazt tudja

Ezekhez erdemes megnezni ezt a [feature matrix](http://damagecontrol.codehaus.org/Continuous+Integration+Server+Feature+Matrix)ot.

Meg pl a munkahelyem is irt sajatot, az is eleg jo, es persze van tucat mas belso fejlesztes meg kereskedelmi cucc.

Mit is tud egy ilyen eszkoz:

*   Ismeri a [version control](version%20control.html) rendszeredet
*   Estenkent kicsekoutol, lebuildel fullra
*   Teszteket is lefuttatja (peldaul [junit](junit.html))
*   Amikor becommitolsz valamit akkor is figyelhet. (bar ez ritkabb mert eroforrasigenyesebb)
*   A [build](build.html) outputot es a teszteredmenyeket kikuldi a megfelelo cssatornakra (mail, [irc](irc.html), [IM](Missing.html), miegymas)
*   Es persze mindehhez gyonyoru szep feluletet is biztosit.
*   Mos, foz, takarit, megmenti a vilagot, neked mar telleg csak a kodot kell irnod

Cikkek:

*   [Automation for the people: Continuous feedback](http://www.ibm.com/developerworks/java/library/j-ap11146/index.html?ca=drs-)
*   [Which open source CI tool is best suited for your application's environment?](http://www.javaworld.com/javaworld/jw-11-2006/jw-1101-ci.html) (review: Cruise Control, Continuum, Luntbuild, Hudson)
*   [Introducing continuous integration  ](http://www.javaworld.com/javaworld/jw-06-2007/jw-06-awci.html)

Lasd meg: [XP](XP.html)



