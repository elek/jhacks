---
creationDate        : 2007-06-06 16:12:23 +0200 
author              : kocka 
title               : perforce 
name                : perforce 
layout              : wiki 
path                : perforce 
date                : 2008-03-31 12:15:20 +0200 
version             : 10 
creator             : kocka 
---
[http://www.perforce.com/](http://www.perforce.com/)

Egy [version control](version%20control.html) rendszer, multiplatform. Nem szabad, de [free](Open%20Source.html) szoftverekhez ingyen lehet használni. Van hozzá [eclipse](Eclipse.html) [plugin](http://www.perforce.com/perforce/products/p4wsad.html), command line és grafikus kliens, webes kliens, proxy elé, meg egyéb kütyük.

*   Érdekes baleset vele például egy directory letörlése, mert ahhoz a workspace-det kell módosítani úgy, hogy az ténzleg törölje. Vicces.
*   Összehasonlításként az sync (az svn up megfelelője) kb ugyanolyan fürge mint a svn-ben, viszont ezerszer gyorsabb mint a VSS. Ez most így tudománytalanul...
*   Tréfás dolog a kliens workspace is. A p4 nyilvántartja hogy ki szedte le a forráskódot és melyik gépről, és csak arról a gépről engedi újra azzal a kliens workspace névvel sync-elni. Ha esetleg letörölted a teljes forrásfát, na akkor egy 'p4 client -d -f myworkspace' paranccsal lehet rendet tenni, ami letörli azt amit már kézzel amúgy is :) Az is hasonló eset, amikor DHCP szerver vagy a vicces rendszergazda új IP címet vagy gépnevet oszt ki, na akkor is bukod a kliensedet teljesen.
*   Kicsit sokmindent nem lehet megcsinálni az egyébként tréfás grafikus kliensekről, például a directory törlést sehogy sem sikerült...
*   Ha pl 'rm -rf'-fel letörölted a forrsáfa egy részét és szeretnéf mégis visszakapni, hát akkor izé... Mind1, ilyet ne csinálj!
*   Sajnos az eclipse plugin időnként nem hozza fel a legfrissebb verziót a 'sync to head' parancsra, csak rátesz egy kis sárga ikont hogy nem a egfrissebb. Ezt elég nehéz észrevenni és kicsit erőszakoskodni kell vele hogy elmúljon. Nem valami barátságos.
*   Na még egy izgalmas részletet mesélnék erről a zseniális szoftverről: Amikor licenszeled (annyiba kerül hogy ennyiért már felvehetnél egy programozót úgy fél évre), akkor a szervered IP-címére kell a licenszt kérni, így amikor valamilyen technikai okból a szerver IP-címe változik, akkor bizony interakcióba kell lépni a sales team-mel és új licenszt kérni hozzá. Közben az ember azon gondolkodik, hogy ennyi idő alatt hányszor [migrált volna át](http://p42svn.tigris.org/) [subversionra](subversion.html) :-)

Szóval mindent összevetve, elég érdekes dolog, és nem túl szórakoztató hosszútávon. Aki mégis a kijárt utat akarja járni, az talán jobban jár a [subversion](subversion.html)nal :)

Talán leginkább a [ClearCase](ClearCase.html) hasonlít rá. - az se volt soha a szivem csücske :-)


