---
creationDate        : 2005-11-28 15:50:29 +0100 
author              : admin 
title               : WTF/Cancel button 
name                : WTF/Cancel button 
layout              : wiki 
path                : WTF/Cancel button 
date                : 2006-03-26 01:43:01 +0100 
version             : 1 
creator             : kocka 
---
Na kozzetennek egy sajat gyartamanyomat is :)

Egyszer [swing](../Swing.html)es [gui](../gui.html)kat gyartottunk egy ugyfelnek, persze mindig utaltam a [ui](../Missing.html) dolgokat, ugyhogy, meg akkor meg nem volt [Eclipse/Plug-in/Visual Eclipse](../Eclipse/Plug-in/Visual%20Eclipse.html) plugin az [eclipse](../Eclipse.html)ben, ugyhogy nem kavartunk tul sokat :)

A gui a kovetkezokeppen nezett ki: beviteli mezok, alul egy 'OK' gomb ami az [adatbazis](../Adatbazis.html)on a megfelelo modositast vegrehajtotta. Az ugyfel jott hogy na jo de mi legyen ha meggondolja magat es nem akarja vegrehajtani a dolgot? Erre en mondtam hogy akkor ne nyomja meg a gombot.

Mindegy, nem dobta fel oket az otlet, taskkent ki lett osztva hogy legyen akkor is egy  'cancel button', meg aznap meg is lett :) Igy az 'OK' gomb megnyomasara az adat bekerult az adatbazisba mig a 'Cancel' gomb megnyomasara __nem__ kerult be.

Aztan jott megint a juzer tesztelni, (ez ilyen [on-site customer](../on-site%20customer.html) volt) megnyomta boldogan a 'Cancel' gombot es az adat nem kerult az adatbazisba, siraj, viszont hibakent megjegyezte hogy az ablak ottmaradt :)

Hat ennyit permi patternjerol a 'Cancel' gombok egeszen sajatos mukodeset illetoen :) 
