---
creationDate        : 2004-11-19 13:11:04 +0100 
author              : kocka 
title               : james 
name                : james 
layout              : wiki 
path                : james 
date                : 2005-07-12 19:53:48 +0200 
version             : 4 
creator             : kocka 
---
__James__, a Java Mail Server

[http://james.apache.org/](http://james.apache.org/)

Egy konnyed bucsu a buffer overflow tamadasoktol. Klassz kis absztrakt komponensarchitekturaja van, ugyesen lehet a [j2ee](j2ee.html) azonositasi rendszerbe integralni, vagy adatbazist pakolni a segge ala. Szoval franko kis cucc. [avalon](avalon.html) alapu mellesleg, [phoenix](phoenix.html)-en fut, elmeletileg [loom](loom.html)-on is.

A POP3 es az SMTP protokollokat tamogatja, nagyon kellene valaki eki implementalna az IMAP protokolt.

Pár hozzá csatlakozó project, ki tudja mikor jön jól majd:

*   [http://jvgroups.sourceforge.net/](http://jvgroups.sourceforge.net/) Levlista menedzselő webapp [James](james.html)-hez
*   [http://sourceforge.net/projects/james-ha/](http://sourceforge.net/projects/james-ha/) Valamiféle clusterezés, fail-over, meg ami kellhet, ha már egy VM nem birja...

Folyamatban:

*   Fast fail support (ne kerdezd hogy mi az, nem tudom valami belso cucc)
*   [Avalon](avalon.html) fuggetlenites. Ettol nem lesz jobb semmi.
*   Admin [webapp](webapp.html). A [JMX](JMX.html) cuccokat nem eroltettek tul, kivancsi vagyok hogy milyen lesz a webapp...
