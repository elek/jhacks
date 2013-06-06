---
creationDate        : 2007-09-27 15:12:44 +0200 
author              : karenin 
title               : Design Patterns/Creational Patterns/Prototype 
name                : Design Patterns/Creational Patterns/Prototype 
layout              : wiki 
path                : Design Patterns/Creational Patterns/Prototype 
date                : 2007-09-27 15:12:44 +0200 
version             : 1 
creator             : karenin 
---
A prototype minta arra akar emlékeztetni minket, hogy ha egy bűn lassú konstruktorunk van (pl. feltölti az osztály változóit valami nagyon messzi adatbázisból), akkor gondolkozzunk el rajta, hogy nem-e érdemes inkább a már felépített osztályt (ez lenne a prototípus) klónozni (mármint a lassú konstruktort nem le futtatni, csak az osztályváltozókar másolgatni.) Persze ehhez az kell, hogy a bűn lassú adatbázis ritkábban változzon, mint ahogyan mi objektumot szeretnénk belőle szerezni.
