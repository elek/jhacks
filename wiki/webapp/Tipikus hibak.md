---
creationDate        : 2005-03-28 22:58:12 +0200 
author              : kocka 
title               : webapp/Tipikus hibak 
name                : webapp/Tipikus hibak 
layout              : wiki 
path                : webapp/Tipikus hibak 
date                : 2005-03-28 23:48:23 +0200 
version             : 5 
creator             : kocka 
---
En tipikus [webapp](../webapp.html) hibanak tartom azt, amikor valaki annak ellenere hogy valojaban nincs szuksege tobbre mint amennyit a [servlet](../servlet.html) container vagy [j2ee](../j2ee.html) [alkalmazas szerver](../Alkalmazas%20Szerver.html) egyebkent is szolgaltat, megis sajat megoldas kerul implementaciora a [webapp](../webapp.html)ban.

A dolog egyetlen elonye az, hogy egyszeru esetekben konnyebb feltelepiteni az alkalmazast, viszont hatranya nagyon sok van:

*   Az azonositasi rendszer nem integralhato ossze (legfeljebb talan az [RDBMS](../RDBMS.html) retegben, de erre halvany az esely)
*   Az adatbazis mozgatasokat nehezen turi.
*   Eroforras optimalizacio szinte nincs is.
*   Nem is valami megbizhato.

Amibol ezt a listat osszeallitottam: [Drone](../drone.html), [snipsnap](../SnipSnap.html), [scarab](../scarab.html) es egyebek.

Lasd meg: [webapp/db connection pool](../webapp/db%20connection%20pool.html)
