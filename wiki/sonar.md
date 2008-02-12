---
creationDate        : 2008-02-12 21:27:17 +0100 
author              : kocka 
title               : Sonar 
name                : sonar 
layout              : wiki 
path                : sonar 
date                : 2008-02-12 21:31:10 +0100 
version             : 2 
creator             : kocka 
---
[http://sonar.hortis.ch/](http://sonar.hortis.ch/)

Egy aggregátor [checkstyle](checkstyle.html), [pmd](PMD.html), cobertura és surefire elé, valamint a hozzá passzolo [adatbázis](RDBMS.html) frontent [webapp](webapp.html). Alapból [mavennel](maven/maven2.html) muzsikál együt, de [ant](ant.html) projectekre is rá lehet kényszeríteni.

A dologban szépségei:

*   Nem kell módisítani a pom.xml-t.
*   Egy biztos helyen([RDBMS](RDBMS.html)) van a QA statisztika, onnan lehet riportolni is

A felgyűlt statisztikát időben és pillanatképként is nézhetjük. Szóval hasznos kis cucc...

Lásd még: [Continuous Integration](Continuous%20Integration.html), [QALab](qalab.html)


