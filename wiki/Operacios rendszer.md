---
creationDate        : 2005-01-06 14:25:53 +0100 
author              : admin 
title               : Operacios rendszer 
name                : Operacios rendszer 
layout              : wiki 
path                : Operacios rendszer 
date                : 2006-03-26 01:42:48 +0100 
version             : 1 
creator             : kocka 
---
Mint azt a versenyhivatlatol megtudtuk:
Harom fajtaja ismert: [Microsoft](Microsoft.html), [Linux](Linux.html) es [IBM](IBM.html) :D

# Benchmarkok, tuningok

*   [http://www.spindazzle.org/benchmarks/](http://www.spindazzle.org/benchmarks/)
*   [http://java.sun.com/j2se/1.4.2/1.4.2_whitepaper.html](http://java.sun.com/j2se/1.4.2/1.4.2_whitepaper.html)

# Java operacios rendszerek (kiserlet)

*   [http://jnode.org](http://jnode.org)
*   [http://JBox.dk](http://JBox.dk)
*   [http://www.jxos.org/](http://www.jxos.org/)

Valamint megemlitendo a [sun](Sun.html) [java desktop system](Missing.html)-e, ami nagyon szep, de gyakorlatilag egy [linux](Linux.html)+gnome, jopar java programmal telenyomva.

# Oprendszer fuggoseg

Bar ketsegtelenul nem kis idiotizmus szukseges a dologhoz, [java](java.html)ban is lehet irni operacios rendszer fuggo kodot, nehany gyakori megoldas:

*   [windows](Windows.html) pathok hardcode-olasa (lehetne akar egy [WTF](WTF.html) is)
*   [JNI](JNI.html) csak ugy

Az olyan dolgokkal is lehet neheziteni a dolgot, hogy pl [awt](AWT.html)t vagy a ra epulo [swing](Swing.html)et hasznalod fel szerver oldali komponensekben, tipikusan [servlet](servlet.html)ekben. Tokre sux mert [linux](Linux.html) szervereken tipikusan nem fut X11, igy az el fog halni. Futaskornyezetet kell patchelni meg minden. Szoval fajni fog.
