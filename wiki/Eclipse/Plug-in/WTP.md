---
creationDate        : 2005-06-16 19:35:23 +0200 
author              : kocka 
title               : Web Tools Project 
name                : Eclipse/Plug-in/WTP 
layout              : wiki 
path                : Eclipse/Plug-in/WTP 
date                : 2006-07-31 17:49:41 +0200 
version             : 9 
creator             : kocka 
---
Az [Eclipse](../../Eclipse.html) [j2ee](../../j2ee.html) support pluginjat szolgaltato project. Erezheto rajta az [IBM](../../IBM.html) [Websphere app dev](../../Websphere%20App%20Dev.html) stilusa, pontosabban abbol forkolhattak ki. Mar hasznosnak bizonyult [tomcat](../../tomcat.html)es [webapp](../../webapp.html) projectek eseten, eleg konnyen lehet hozzakezdeni, csak megint valami specialis directory strukturat tamogat, pl [maven](../../maven.html)nel mar nem esne jol. Azert erdemes hasznalni.

Kulonosen szeretnivalo a [tomcat](../../tomcat.html) integraciojaban peldaul az, hogy a [tomcat](../../tomcat.html) config allomanyait (server.xml es opcionalisan a tomcat-users.xml) a Servers project mappaiban tartja, igy egyszeruen el tudod erni es [xml](../../XML.html) editorral modosithatod ami nem tetszik benne. __Szivasok__: Hat tart egy kis redundanciat az [eclipse](../../Eclipse.html), ez nem is lenne baj, csak idonkent szejjelcsuszik az egesz. Pl amikor editalod a [tomcat](../../tomcat.html)od koncif allomanyait, es csak nem mukodik a dolog, akkor valoszinuleg errol van szo. Meg idonkent mintha baja lenne a classpath-hal is.

![image](http://www.jhacks.hu/space/Eclipse/Plug-in/WTP/wtp-2005-09-29.gif)
_Egy kepernyoloves a szebb ficsorokkel: [jsp](../../JSP.html) editor, servers view, outline_

__Hibak:__

*   A beepitett browser ami valojaban valoszinuleg a default mozilla/firefox agyoncsapaja a VM-edet ha kap egy 401-et es megprobalja felpopupolni az azonositasi ablakot.
*   [weblogic](../../weblogic.html) 8.1-gyel nem igazan akar mukdoni pla deploy.
*   meg sok mas, gondolom, csak ebbe nagyon belebotlottam.

![image](http://hackers.forgeahead.hu/space/Eclipse/eclipse-31m5wtp.png)
_ Ezt a kepet meg akkor csinaltam amikor nagyon gebasz volt a WTP, majd lecserelem valami frissebbre valmikor. Rugdossatok :) _
