---
creationDate        : 2004-08-20 00:12:41 +0200 
author              : kocka 
title               : log4j 
name                : log4j 
layout              : wiki 
path                : log4j 
date                : 2005-06-12 16:01:53 +0200 
version             : 4 
creator             : kocka 
---
![image](http://logging.apache.org/log4j/docs/images/logo.jpg)(http://logging.apache.org/)

A Log4j a jdk 1.4 elotti idokbol szarmazik, amikor meg nem volt [logging](Logging.html) a javaban. Annyira bevallt, hogy szinte minden framework es [alkalmazas szerver](Alkalmazas%20Szerver.html) hasznalja, vagy tamogajta valahogy a hasznalatat. Kar hogy nem a log4j lett jsr :(

Elonyei:

*   Rugalmas: sokfele appender van hozza, sokfelekeppen lehet konfiguralni (xml, propertyfile, stb, vagy amit irsz hozza :) )
*   Biztonsagos: a loging rendszer nem dob hibat, igy ha a rendszerben csak a logging konfigot szurtad el meg mindig megy a szoftvered.

Nagyon hasznos [eclipse](Eclipse.html) tool hozza a [log4e](log4e.html), amivel az idiota System.out.println()-eket tudod ket kattintassal atirni loggingra.

Beepitett appenderek:

*   [socket](Missing.html)
*   [rdbms](RDBMS.html)
*   file
*   [jms](JMS.html)
*   (ennyi jutott eszembe meg van tucatnyi azert :) )

Appenderek mas projectekben:

*   [log4rss](log4rss.html)
*   [hibernate](Hibernate.html)
*   A [PL-J](PL-J.html) is tartalmaz egy appendert, ami az adatbazis logjaba kuldi az uzeneteket
*   [jabber](jabber.html) [http://www-106.ibm.com/developerworks/java/library/j-instlog/](http://www-106.ibm.com/developerworks/java/library/j-instlog/)

Tucat port keszult a log4j tervezesi mintai alapjan mas programozasi nyelvekre: C++, php, python.

[Renszarv](renszarv.html) monda vala:<br/>
Hát amikor elkezdtem az ipart, akkor java-ból 1.2.2 volt a tuti, a log4j org.log4j packageben volt és nem org.apache.log4j-ben, (sőt, volt még com.ibm.log4j-s verzió is :) )
