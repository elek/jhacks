---
creationDate: 1190897733895 
author: karenin 
contentAuthor: karenin 
title: Design Patterns/Creational Patterns/Builder 
contentUpdateDate: 1190897982009 
name: Design PatternsCreational PatternsBuilder 
layout: wiki 
date: 1190897982009 
creator: karenin 
---
Egyike azoknak a mintáknak ameylek annyira alacsony szintűek, hogy nagyon magyarázni kell, hogy miért is minták.

A szakirodalom szerint arra jó, hogy elválasztjuk egymástól egy objektum létrehozásást attól, hogy milyen is egy ilyen objektum.

Ehhez is kell egy interface, amiben mindenféle okos függények vannak. És van egy Director osztályunk, ami kap egy ilyen intarface-nek megfelelő osztályt, és az okos fügvényeket használja. (pl. felépíthet ezeknek segítségével egy fát, innen a Build név, de szerintem bármi mást is csinálhat). Persze mielőtt a Build osztálnyak átadjuk az interface implementációját, már létrehoztuk, de ez egy másik történet (na itt a szétválasztás).

Szóval vagy az van, hogy én nagyon nem értem a minta lényegét, vagy ez igazából az, amit mindenki használ, hogy interface-ektől függünk, nem implementácioktól, csak éppen ojjektum építésekor használva.

A tipikus példa az szokott lenni, amikor csináluk mondjuk egy DOM fát, de akár többfajta reprezentációból (pl. XML, FastInfoset). Ekkor több Builder interfaceünk van, de a Director mindegyikbű ugyanazt látja (pl. hogy kérem a következő tokent, meg hogy van-e még), és nem kell azzal foglalkozni, hogy milyen reprezentációba érzekett az adat.
