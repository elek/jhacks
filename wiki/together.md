---
creationDate: 1091021869581 
author: kocka 
contentAuthor: kocka 
title: together 
contentUpdateDate: 1112882405432 
name: together 
layout: wiki 
date: 1112882405432 
creator: kocka 
---
Egy csili vili UML designer a [borland](borland.html)tol.

Van belole free verzio (as beer), es funkcionalisan eleg jo.

Elso blikkek:

![Screenshot](Screenshot-1.png)(http://hackers.forgeahead.hu/space/together/Screenshot-1.png)<br/>
_ Screenshot Red hat 9-en, eppen classdiagram tervezes kozben: ezerszer gyorsabban hasznalhato mint az ArgoUML_


Nagyon is jo, meg intuitiv a felulete. Ha az ember ismeri az [UML](UML.html) diagrammokat, akkor gyorsan es egyszeruen... Ami pozitivum, hogy kepes kezelni az [UML](UML.html) 2.0 diagramjait is es van benne egy normalis ER diagram editor.

![Screenfuck by Golyo](ER_Diagram.JPG)(http://hackers.forgeahead.hu/space/together/ER_Diagram.JPG)
_ ER diagram<br/>Itt szepen latszik, hogy az az alat ugy csinal, mintha a tabla egy view lenne es minden kulcs jellegu dolgot delegal a tablaba... _

Ami viszont problem:

# Altalaban:

*   Az ER diagrammon szepen megcsinalja az foreign keyeket amikor egy kapcsolatot hozol letre. Viszont, ha olyan tabalara linkelsz, aminek tobb kapcsolata is van, akkor nem altal az osszes FK-t breakni attributumnak... vazzzz. (Na jo, ha ugy vesszuk, akkor mutatja a FK-eket. Ertelmezes kerdese. Kiderulni nem fog, hogy melyik, mert ugy tunik kodot nem lehet vele generalni... Kep mellekelve. Szerintetek ez atlathato?)

# Linux:


A [windows](Windows.html)os verzio szuper, meg jo. Ellenben a [Linux](Linux.html)-os verzioval vannak gondok. Elsore azt hittem en vagyok a hulye, de ra kelett jonnom, nem. Szoval a bugok:
*   A helo systembe csak ugy tudsz bemenni, ha a folinkre pozicionalsz, majd megnyomod a 'Next Topic' gombot. Mondanom sem kell, hogy W$ alatt, ez duplaklikkre megy.
*   Az elozo meg hagyjam, de a masik bug amit talaltam, az az, hogy egyszeruen nem lehet elovarazsolni a diagram editort. Elvileg rogton meg kene nyilnia, ha egy uj diagramot csinalsz, vagy megnyitsz egyet, (W$ alatt meg is tortenik persze...) de Linux alatt egyszeruen nem megy... VAZZ!!! (Annyi tennek hozza, hogy megy, de csak akkor, ha root-kent futtatom (Slackware 10.0))
