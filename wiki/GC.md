---
creationDate: 1093859596968 
author: kocka 
contentAuthor: kocka 
title: GC 
contentUpdateDate: 1126102067168 
name: GC 
layout: wiki 
date: 1126102067168 
creator: kocka 
---
__Garbage Collector__

A GC tulajdonkeppen nem egy [java](java.html) specifikus modszer, hanem egy viszonylag uj (ehh, alig 10-20 eves) programozasi koncepcio.

__A problema:__ A programozok gyakran feledkeznek meg az allokalt memoria felszabaditasarol, sokszor az sem tisztazott hogy melyik programnak kell felszabaditania a memoriateruletet. Gyakran keletkezik [memory leak](memory%20leak.html). 

__A megoldas:__ A GC megszabaditja a programozokat a memoriakezeles problemajatol. A programozo egyszeruen csak kodol, es a lefoglalt memoriat a rendszer nyilvantartja, es egy kulon szolgaltatassal foglalkozik vele. Extra: a felhasznaloi keres kiszolgalasakor nem kell a memoriafelszabaditassal foglalkozni, raer kesobb is.

__Keletkezett problema:__ A hulyesegre nincs orvossag, ha a az alkalmazasodbol megis hagysz hivatkozast egy objektumra, peldaul egy statikus listaban, akkor nem fog torlodni. (a [memory leak](memory%20leak.html) keletkezesenek altalanos es gyakori oka)

A GC megfelelo beallitasa kulcskerdes az optimalis sebesseg eleresehez. (ugyanis a GC leallitja a VM-ed futasat egy idore)

olvasnivalo:

*   http://java.sun.com/docs/hotspot/VMOptions.html
*   http://java.sun.com/docs/hotspot/gc1.4.2/index.html



Erdemes a forrast is elolvasni, erdekes dolgok derulnek ki.



Lasd meg: [OOM](OOM.html), [memory leak](memory%20leak.html)




