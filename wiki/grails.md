---
creationDate        : 2006-10-13 11:06:04 +0200 
author              : kocka 
title               : grails 
name                : grails 
layout              : wiki 
path                : grails 
date                : 2007-01-14 07:37:12 +0100 
version             : 8 
creator             : kocka 
---
![image](http://www.grails.org/images/grails_logo.jpg)(http://www.grails.org/)

Avagy [groovy](Groovy.html) on rails.

Egy [rad](rad.html) [webapp](webapp.html) alkalmazas fejleszto eszkoz, [hibernate](Hibernate.html), [spring](spring.html), [quartz](quartz.html), stb integracioval. Szoval minden ami altalaban kellhet, az oldalakat [gsp](Missing.html)ben irhatod, a controllereket meg [groovy](Groovy.html)ban.

Van benne egy kis [jetty](jetty.html) is, szoval minden meg rajta egybol.

Hat, kiprobalva gyorsan: igen tenyleg mukodik egy gyors apro fejlesztesben, de tobbet nem tudok mondani. Ha valaki csinalt vele nagyobb komolyabb dolgot keretik nyilatkozni :)

Nehany funkcio:

*   [test](test.html)ek tamogatasa, [functional testing](functional%20testing.html) ([canoo](canoo.html))
*   alapbol az [eclipse](Eclipse.html)hez general project es classpath fileokat

Faraszto dolgai:

*   valami furcsa modon hasznalja a [spring](spring.html)-et, persze sima [dbcp](DBCP.html) datasource-ot startol fel amit a franko kis [groovy](Groovy.html)s config objektumaival inicializal, CSAKHOGY ezt a datasource-ot nem fogod tudni elerni az applicationContext.xml-be pakolt objektumokbol mert egy al-contextben van. Ezt nem tudom miert kell igy csinalni de letezo service osztalyok integralasa ([dao](DAO.html) foleg) innentol kezdve eleg cikis.
*   nincs belenyomva a tranzakcio kezeles, azzal is harcolni kell
*   [ajax](ajax.html) tamogatas: [laszlo](Laszlo.html) inbtegracio egyetlen [ant](ant.html) paranccsal


