---
creationDate        : 2007-06-06 16:12:23 +0200 
author              : kocka 
title               : perforce 
name                : perforce 
layout              : wiki 
path                : perforce 
date                : 2008-01-17 14:07:14 +0100 
version             : 5 
creator             : kocka 
---
[http://www.perforce.com/](http://www.perforce.com/)

Egy [version control](version%20control.html) rendszer, multiplatform. Nem szabad, de [free](Open%20Source.html) szoftverekhez ingyen lehet használni. Van hozzá [eclipse](Eclipse.html) plugin, command line és grafikus kliens, webes kliens, proxy elé, meg egyéb kütyük.

*   Érdekes baleset vele például egy directory letörlése, mert ahhoz a workspace-det kell módosítani úgy, hogy az ténzleg törölje. Vicces.
*   Összehasonlításként az sync (az svn up megfelelője) kb ugyanolyan fürge mint a svn-ben, viszont ezerszer gyorsabb mint a VSS. Ez most így tudománytalanul...
*   Tréfás dolog a kliens workspace is. A p4 nyilvántartja hogy ki szedte le a forráskódot és melyik gépről, és csak arról a gépről engedi újra azzal a kliens workspace névvel sync-elni. Ha esetleg letörölted a teljes forrásfát, na akkor egy 'p4 client -d -f myworkspace' paranccsal lehet rendet tenni, ami letörli azt amit már kézzel amúgy is :)
*   Kicsit sokmindent nem lehet megcsinálni az egyébként tréfás grafikus kliensekről, például a directory törlést sehogy sem sikerült...

Akik megis a kijart utat akarjak jarni azok talan jobban jarnak a [subversion](subversion.html)nal :)

Na még egy izgalmas részletet mesélnék erről a zseniális szoftverről: Amikor licenszeled (annyiba kerül hogy ennyiért már felvehetnél egy programozót úgy fél évre), akkor a szervered IP-címére kell a licenszt kérni, így amikor valamilyen technikai okból a szerver IP-címe változik, akkor bizony interakcióba kell lépni a sales team-mel és új licenszt kérni hozzá. Közben az ember azon gondolkodik, hogy ennyi idő alatt hányszor migrált volna át [subversionra](subversion.html) :-)


