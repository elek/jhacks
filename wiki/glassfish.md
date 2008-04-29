---
creationDate        : 2005-06-13 16:14:04 +0200 
author              : karenin 
title               : glassfish 
name                : glassfish 
layout              : wiki 
path                : glassfish 
date                : 2008-04-29 20:16:07 +0200 
version             : 10 
creator             : kocka 
---
![image](http://glassfish.dev.java.net/public/image/glassfish_logo.gif)(http://glassfish.dev.java.net/)


-   [glassfish](glassfish.html)



A [SUN](Sun.html) egy community [j2ee](j2ee.html) 1.5 [alkalmazas szerver](Alkalmazas%20Szerver.html)e. (Kereskedelmi nevén Sun Java System Application Server. A SUN érdekes névadási és verziózási konvenciója miatt a Glassfish V2 az a Sun Java System Application Server 9.1.)

Erdekes ujitasok:

*   [NIO](NIO.html) alapu [HTTP](HTTP.html) listener (Grizzly)
*   lazy initialization, csak azokat a szolgaltatasokat inditja el, amire szukseg van (v3)
*   Glassfish news blog: [http://blogs.sun.com/theaquarium](http://blogs.sun.com/theaquarium)

Verziók:

*   v1 a múzeumból
*   v2 jelenleg ez a stabil, főleg clusterezésben újabb, az admin felület JSF-es ilyenek
*   v3 teljesen új architektúra ([HK2](HK2.html) és [OSGi](OSGi.html)). Moduláris lesz, ezért állítólag alapból kevesebb erőforrást eszik. Támogatni fogja a szkript nyelveket, és beágyazott módban is lehet majd indítani (érts Java kódból).
