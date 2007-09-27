---
creationDate        : 2007-09-27 14:55:33 +0200 
author              : karenin 
title               : Design Patterns/Creational Patterns/Builder 
name                : Design Patterns/Creational Patterns/Builder 
layout              : wiki 
path                : Design Patterns/Creational Patterns/Builder 
date                : 2007-09-27 14:55:33 +0200 
version             : 1 
creator             : karenin 
---
Egyike azoknak a mintáknak ameylek annyira alacsony szintűek, hogy nagyon magyarázni kell, hogy miért is minták.

A szakirodalom szerint arra jó, hogy elválasztjuk egymástól egy objektum létrehozásást attól, hogy milyen is egy ilyen objektum.

Ehhez is kell egy interface, amiben mindenféle okos függények vannak. És van egy Build osztályunk, ami kap egy ilyen intarface-nek megfelelő osztályt, és az okos fügvényeket használja. (pl. felépíthet ezeknek segítségével egy fát, innen a Build név, de szerintem bármi mást is csinálhat). Persze mielőtt a Build osztálnyak átadjuk az interface implementációját, már létrehoztuk, de ez egy másik történet (na itt a szétválasztás).

Szóval vagy az van, hogy én nagyon nem értem a minta lényegét, vagy ez igazából az, amit mindenki használ, hogy interface-ektől függünk, nem implementácioktól.
