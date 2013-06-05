---
creationDate: 1118672044101 
author: karenin 
contentAuthor: karenin 
title: glassfish 
contentUpdateDate: 1209492978219 
name: glassfish 
layout: wiki 
date: 1209492978219 
creator: kocka 
---
![image](http://glassfish.dev.java.net/public/image/glassfish_logo.gif)(http://glassfish.dev.java.net/)



A [SUN](Sun.html) egy community [j2ee](j2ee.html) 1.5 [alkalmazas szerver](Alkalmazas%20Szerver.html)e. (Kereskedelmi nevén Sun Java System Application Server. A SUN érdekes névadási és verziózási konvenciója miatt a Glassfish V2 az a Sun Java System Application Server 9.1.)

Erdekes ujitasok:

*   [NIO](NIO.html) alapu [HTTP](HTTP.html) listener (Grizzly)
*   lazy initialization, csak azokat a szolgaltatasokat inditja el, amire szukseg van (v3)
*   Glassfish news blog: http://blogs.sun.com/theaquarium



Verziók:

* v1 a múzeumból

* v2 jelenleg ez a stabil, főleg clusterezésben újabb, az admin felület JSF-es ilyenek

* v3 teljesen új architektúra ([HK2](HK2.html) és [OSGi](OSGi.html)). Moduláris lesz, ezért állítólag alapból kevesebb erőforrást eszik. Támogatni fogja a szkript nyelveket, és beágyazott módban is lehet majd indítani (értsd Java kódból).
