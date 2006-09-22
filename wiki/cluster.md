---
creationDate        : 2004-12-08 11:30:19 +0100 
author              : kocka 
title               : cluster 
name                : cluster 
layout              : wiki 
path                : cluster 
date                : 2006-09-22 22:54:27 +0200 
version             : 5 
creator             : kocka 
---
__Cluster__

A clusterezes az az amikor az alkalmazasod tobb szerveren fut, persze annelkul hogy errol tulajdonkeppen tudomasa lenne. A cluster [session failover](session%20failover.html)t es [load ballancing](load%20ballancing.html) szolgaltatasokat biztosit, ezt persze az [alkalmazas szerver](Alkalmazas%20Szerver.html)nek kell megoldania.

A cluster nem mindig hoz megvaltast. Pl ha tul sok az adat a juzer session-jaban, akkor tul sok idobe tellik szinkronban tartani tobb szerveren. Persze van amikor viszont pl bejelentkezes soran felolvasod a falhsznalo adatait adatbazisbol es meg mindig jobb a cluster par nodja kozott replikalni mint az adatbazist foloslegesen terhelni vele minden request kiszolgalasakor. Bar az adatbazis terheles enyhitesere is ezer mas megoldas van mar. Szoval ingovanyos terulet, csinald ahogy jonak latod :)

A clusterek masik fajtaja a szamitasi cluster, ezt nem a magunkfajta hegesztomunkas hasznalja hanem a muveltebb emberek. Fizikusok, biologusok, vegyeszek, ilyesmi, ezen a teruleten az MPI uralkodik meg mindig.
