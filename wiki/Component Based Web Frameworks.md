---
creationDate        : 2007-09-19 15:51:16 +0200 
author              : karenin 
title               : Component Based Web Frameworks 
name                : Component Based Web Frameworks 
layout              : wiki 
path                : Component Based Web Frameworks 
date                : 2007-09-19 15:51:16 +0200 
version             : 1 
creator             : karenin 
---
Nem tudom van-e valami olyan neve ezeknek a dolgoknak, mint az [MVC](MVC.html). Ezek a cuccok igazából az [MVC](MVC.html)-t váltják, egyre jobban divatba jönnek. Valami olyasmi a lényege, hogy a webalkalmazást már nem úgy írunk, hogy a bejön a request és kimegy a response, hanem inkább egy kicsit Swinges mentaláitással, hogy felépítünk egy komponens fát, és majd a komponenesek kezelik a saját birodalmukon a kéréseket.

Elég kényelmes dolgokat lehet csinálni, pl. elvileg külön komponeneseket árulni és azokat egyszerűen újrahsznosítani.

Persze mindennek ára van, a komponens fának minden requesthez létezni kell, ezért vagy mindig fel kell építeni (pl. [JSF](JSF.html)) vagy session-ba kell tárolni a serializálható részét (pl. [Wicket](Wicket.html)). Vagy ezt a kettőt keverhetjük akár a fentiekben is.

Frameworkok:

*   [JSF](JSF.html) a szabványos
*   [Wicket](Wicket.html) az ifjú titán
*   [tapestry](tapestry.html) a nagy öreg
