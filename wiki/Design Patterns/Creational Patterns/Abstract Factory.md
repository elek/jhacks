---
creationDate: 1190894925834 
author: karenin 
contentAuthor: karenin 
title: Design Patterns/Creational Patterns/Abstract Factory 
contentUpdateDate: 1190894925834 
name: Design PatternsCreational PatternsAbstract Factory 
layout: wiki 
date: 1190894925834 
creator: karenin 
---
A tipikus példa amit erre szoktak mondani az a LookAndFeel készletek. Kell kettő vagy több ostálykészlet (Window,Border,stb.), amikből egy készletet szeretnék egyszerre használni (pl. MotifWindow,MotifBorder, stb.)

Megoldás: Csinálunk egy interface-t, aminek vannak createWindow, createBorder, stb. függévnyei, majd implementáljuk két féle képpen. Az egyik ezt a fajta, a másik azt a fajta készletet gyártja le.

Nyilván emiatt a Window is csak egy interface lesz, aminek lesz MotifWindow és GtkWindow megvalósítása is.

Asszem kéne ide rakni egy UML diagramot.
