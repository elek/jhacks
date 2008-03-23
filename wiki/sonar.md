---
creationDate        : 2008-02-12 21:27:17 +0100 
author              : kocka 
title               : Sonar 
name                : sonar 
layout              : wiki 
path                : sonar 
date                : 2008-03-23 09:36:40 +0100 
version             : 7 
creator             : kocka 
---
[http://sonar.hortis.ch/](http://sonar.hortis.ch/)

Egy aggregátor [checkstyle](checkstyle.html), [pmd](PMD.html), cobertura és surefire elé, valamint a hozzá passzolo [adatbázis](RDBMS.html) frontent [webapp](webapp.html). Alapból [mavennel](maven/maven2.html) muzsikál együt, de [ant](ant.html) projectekre is rá lehet kényszeríteni. _(Ilyenkor persze írni kell hozzá egy pom.xml-t mint általában a maven projectekhez és light módban kell futtatni ha a dependency-ket nem töltöttük ki, azaz a tesztek nem futnának és a forrás nem fordulna, ilyesmi)_

A felgyűlt statisztikát időben és pillanatképként is nézhetjük. Szóval hasznos kis cucc...

A dolog szépségei:

*   Nem kell módisítani a pom.xml-t.
*   A fejlesztő szervezet coding policy-ját fel lehet konfigurálni egy központi helyen, ami mellesleg elég felhasználóbarát is.
*   Egy biztos helyen ([adatbázis](RDBMS.html)) van a QA statisztika, onnan lehet riportolni is

A dolog hátulütői:

*   Sajnos az 1.0-ás széria kicsit bétás. A [derby](Derby.html) [adatbázissal](RDBMS.html) elszáll, a [postgresql](PostgreSQL.html)-lel el sem indul, [mysql](MySQL.html)-lel pedig bár megyeget, de rémes hibaüzeneteket dobál setup közben - ami elbizonytalanítja az embert. Nem tudom mit használ perzisztencia rétegként hogy ilyenek vannak. __az 1.1-es verzió sokkal jobb minőségűnek tűnik, most már stabil is__
*   [GPL](GPL.html) és [ruby](ruby.html), túrkálja a forráskódot az akinek nincs jobb dolga :(


Lásd még: [Continuous Integration](Continuous%20Integration.html), [QALab](qalab.html)


