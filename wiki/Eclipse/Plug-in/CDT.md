---
creationDate        : 2005-06-16 19:34:26 +0200 
author              : admin 
title               : Eclipse/Plug-in/CDT 
name                : Eclipse/Plug-in/CDT 
layout              : wiki 
path                : Eclipse/Plug-in/CDT 
date                : 2006-03-26 01:42:38 +0100 
version             : 1 
creator             : kocka 
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
