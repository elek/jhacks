---
creationDate: 1153239346235 
author: kocka 
contentAuthor: kocka 
title: JMeter 
contentUpdateDate: 1153239403768 
name: JMeter 
layout: wiki 
date: 1153239403768 
creator: kocka 
---
([GER](Ger.html) billentyuzetebol, en csak atmasoltam...)<br/>
Habár még sosem teszteltem, de mostanában megismerkedtem a JMeter-rel.

__Leírás:__ apache-os univerzális teljesítmény tesztelő, komponensekből építhetjük fel a teszteket egy GUI segítségével. 

__Komponens típusok:__

*   Thread Group: szálak száma, elindulásuk időzítése és ciklusszámuk megadása
*   Sampler: ez az a valami, amivel tesztelünk. Lehet: [HTTP](HTTP.html), [FTP](FTP.html), [JMS](JMS.html), [LDAP](LDAP.html), [JUnit](junit.html), [Java](java.html) osztály, Mail, [SOAP](SOAP.html), [WebServices](WebServices.html), [JDBC](JDBC.html), stb …
*   Listener: ez az ami gyűjti a tesztadatokat: grafikonok, táblázatok, log fájl, mail, stb…
*   Assertions: ezzel lehet ellenőrizni a rendszertől kapott válaszokat: tartalom, válaszidő, válaszméret, [XML](XML.html) válasz verifikáció/validáció, [XPath](XPath.html), [BeanShell](BeanShell.html) script, MD5, HTML verifikáció
*   Logic Controller: vezérlő szerkezetek, így a kapott válasz függvényében tudunk tesztet végezni (if, while, switch, random, once, stb…)
*   Timer: időzítési szabályok megadása
*   Config Element: konfigurációs beállítások (webauth, cookie, stb…)
*   Pre processors: még a samplerek végrehajtása elött , samplereket modifikáló komponensek: HTML Link Parser, URL rewriting, User parameters, Counter, stb…
*   Post processors: a samplerek eredményét feldolgozó komponensek: reguláris kifejezések, Result status action handler,  stb…



__Előnyök:__
*   Ingyenes
*   Komponens alapú szemlélet
*   Univerzális, komponensek széles választéka, de akár ki is egészíthető
*   Grafikus kezelőfelület, de konzolos üzemmódban is lehet használni automatikus tesztek elvégzésére. Ugyanígy van ant támogatottsága.
*   Vezérlő szerkezetek
*   Változók, paraméterek, funkciók
*   Teszt válasz ellenőrzése
*   Reguláris kifejezések
*   Automatikus URL felvétel egy HTTP Proxy segítségével



__Hátrány:__
*   HTTPS alatt nincsen automatikus URL felvétel
*   Nagyobb teszt közben szinte lehetetlen leállítani, helyette ki kell lőni az egész progit
*   Teszt közben nincsen progress bar, csak indirekt módon lehet következtetni hol jár



__További információ:__
*   http://jakarta.apache.org/jmeter/index.html
*   http://jakarta.apache.org/jmeter/usermanual/index.html
*   http://jakarta.apache.org/jmeter/usermanual/component_reference.html
