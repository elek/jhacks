---
creationDate        : 2004-08-04 11:16:10 +0200 
author              : kocka 
title               : Alkalmazas Szerver 
name                : Alkalmazas Szerver 
layout              : wiki 
path                : Alkalmazas Szerver 
date                : 2006-12-17 23:00:06 +0100 
version             : 9 
creator             : zsoltk 
---
A [J2EE](j2ee.html) arhitektura egyik alapeleme.

Ha megnezzuk a J2EE leirast, akkor tisztan latszik, hogy minden dolog amit hasznalhatunk, egy alkamazas szerver kore epul. Gyakorlatilag a J2EE API es specifikaciot tobbe-kevesbe megvalosito Java program.

Azok a szolgaltatasok amiket egy alkamazas szerver nyujt:

*   [JNDI](JNDI.html)
*   [JMX](JMX.html) es management felulet
*   [Cluster](cluster.html)ing
*   [Servlet](servlet.html) container
*   [EJB](EJB.html)
*   [JTA](JTA.html)
*   [JCA](JCA.html)
*   Resource management, deployment
*   stb

Tipikusan web alkalmazaskohoz hasznaljak, altalaban arra si van kihegyezve, bar ma mar eljutottunk oda, hogy a Kliens - Szerver arhitektura szerver oldali dolgait is meg lehet vele valositani, hiszen rengeteg fele API, Lib es egyeb dolog all rendelkezesunkre.

Az alkalmazas szerver fontos resze a Container, ami egy adott funkciot valosit meg. pld.: [Servlet_jsp](servlet_jsp.html), vagy [EJB](EJB.html).

Az alkalmazas szerverekrol egy osszehasonlito tablazatot lehet a therserverside.com-on talalni: [http://theserverside.com/reviews/matrix.tss](http://theserverside.com/reviews/matrix.tss)

Egy amolyan "Hello World" gyujtemeny, csak eppen itt mashogy hivjak: [petshop collection](petshop%20collection.html)

Nem teljes, de a lenyeget tartalmazo lista:

gyarto|nev|free
[bea](bea.html)|[weblogic](weblogic.html)|developer licensz?
[jboss](jboss.html)|[jboss](jboss.html) as|[LGPL](LGPL.html)
[ASF](ASF.html)|[geronimo](geronimo.html)|[ASF](ASF.html)
[objectweb](objectweb.html)|[jonas](jonas.html)|[LGPL](LGPL.html)
[IBM](IBM.html)|[Websphere](Websphere.html)|3 honap trial
[IBM](IBM.html)|[was-ce](was-ce.html)|tesco-gazdasagos
[sun](Sun.html)|[java system application server](Missing.html)|free verzio
[macromedia](Missing.html)|[jrun](jrun.html)|free download?
[sun](Sun.html)|[glassfish](glassfish.html)|freeware (JRL)



