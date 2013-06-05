---
creationDate: 1118943266048 
author: kocka 
contentAuthor: kocka 
title: Eclipse/Plug-in/CDT 
contentUpdateDate: 1119791277694 
name: EclipsePlug-inCDT 
layout: wiki 
date: 1119791277694 
creator: kocka 
---
__[C](../../C.html) Developement Task__

A Regi CDT egy falabu kis hack volt osszehasonlitva a nagy C/C++ fejlesztokornyezetekkel (KDevelop, Anjuta, satobbi). A jelenlegi verzio egyszeruen angyali kis dolog, szerintem ott van az [eclipse](../../Eclipse.html) erejevel kombinalva mint a tobbi C ide.

Na most meg mielott barki bekepzelne: code completion az hat nincsen igazan (C-ben hogy a turoban lenne :) ). Syntax highlight az meg lehetne valamivel jobb, peldat lehetne venni a [vim](../../VIM.html)rol peldaul.

Ugyanakkor mire is akartam hasznalni: shared objectek debugolasara. Hat ezt nem tudom hogyan lehet vele megtenni, de nem sikerult eddig :(

Nehany screenshot, mert azt szeressuk:

A view-ok, amiket hozzaad az [eclipse](../../Eclipse.html)hez:

![image](CDT-views.gif)(CDT-views.gif)

Lehet a make-t futtatni ugyb hogy a kimenete a konzolra keruljon, igaz nincs sok ertelme, mert az emlitett [C](../../C.html) fejlesztokornyezetekkel ellentetben nem navigalhatoak a hibak.

![image](CDT-PLJ-build.gif)(CDT-PLJ-build.gif)

Ja es szep ikont kapnak a [C](../../C.html) fileok, ez azert kellett mar :)

![image](CDT-PLJ-browse.gif)(CDT-PLJ-browse.gif)

Kovetkeztetes: Olyan fejlesztesekhez mint pl standalone [C](../../C.html) vagy inkabb C++ progik, [JNI](../../JNI.html)s projectek, tok jo. Egyebkent meg mindig a [vim](../../VIM.html)+bash az ami mindent ver.
