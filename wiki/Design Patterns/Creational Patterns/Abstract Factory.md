---
creationDate        : 2007-09-27 14:08:45 +0200 
author              : karenin 
title               : Design Patterns/Creational Patterns/Abstract Factory 
name                : Design Patterns/Creational Patterns/Abstract Factory 
layout              : wiki 
path                : Design Patterns/Creational Patterns/Abstract Factory 
date                : 2007-09-27 14:08:45 +0200 
version             : 1 
creator             : karenin 
---
A tipikus példa amit erre szoktak mondani az a LookAndFeel készletek. Kell kettő vagy több ostálykészlet (Window,Border,stb.), amikből egy készletet szeretnék egyszerre használni (pl. MotifWindow,MotifBorder, stb.)

Megoldás: Csinálunk egy interface-t, aminek vannak createWindow, createBorder, stb. függévnyei, majd implementáljuk két féle képpen. Az egyik ezt a fajta, a másik azt a fajta készletet gyártja le.

Nyilván emiatt a Window is csak egy interface lesz, aminek lesz MotifWindow és GtkWindow megvalósítása is.

Asszem kéne ide rakni egy UML diagramot.
