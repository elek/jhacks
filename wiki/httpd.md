---
creationDate: 1104270100678 
author: kocka 
contentAuthor: kocka 
title: httpd 
contentUpdateDate: 1104270100678 
name: httpd 
layout: wiki 
date: 1104270100678 
creator: kocka 
---
__Apache HTTPD__

Az [ASF](ASF.html) altal fejlesztett Http daemon. A webszerverek piacan a legnagyobb reszesedest a httpd foglalja el.

A nev jelentese `A Pachy http Daemon` (Innen jon az Apache, amirol az alapitvany a nevet kapta). Az elso versioi tenyleg statikisan mokodgettek, majd a nagy elorrelepest jelento 1.3-as szeria modulok (amolyan plugin dolgok) fejleszteset tette lehetove, es egybol tartalmazott is tucat modult: [ssl](Missing.html), [webdav](Webdav.html), azonositasi modulokat, log modulokat, tartalom generalo modulok, stb.

A 2.0-as szeria nagy ujitasa a process/for hibrid uzemmod, amivel jobban passzol az operacios rendszer kepesseigihez.

A [Tomcat](tomcat.html) es a httpd osszecsatolasat a [mod_jk](mod_jk.html) modul vegzi, ez [JNI](JNI.html) hivasokon vagy tcp/ip socketen keresztul kommunikal a tomcat ajp konektoraval. Persze lehet mod_proxy-val is csinalni, de nem tudom abban mi a poen :)
