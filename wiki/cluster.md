---
creationDate: 1102501819837 
author: kocka 
contentAuthor: kocka 
title: cluster 
contentUpdateDate: 1165483220362 
name: cluster 
layout: wiki 
date: 1165483220362 
creator: kocka 
---
__Cluster__

A clusterezes az az amikor az alkalmazasod tobb szerveren fut, persze annelkul hogy errol tulajdonkeppen tudomasa lenne. (Ha megis van tudomasa rola, azt az uzletemberek "custom solution"-nak hivjak, a fejlesztok tuningnak, a felhasznalok meg [tak](tak.html)nak) A cluster [session failover](session%20failover.html)t es [load ballancing](load%20ballancing.html) szolgaltatasokat biztosit, ezt persze az [alkalmazas szerver](Alkalmazas%20Szerver.html)nek kell megoldania.

A cluster nem mindig hoz megvaltast. Pl ha tul sok az adat a juzer session-jaban, akkor tul sok idobe tellik szinkronban tartani tobb szerveren. Persze van amikor viszont pl bejelentkezes soran felolvasod a falhsznalo adatait adatbazisbol es meg mindig jobb a cluster par nodja kozott replikalni mint az adatbazist foloslegesen terhelni vele minden request kiszolgalasakor. Bar az adatbazis terheles enyhitesere is ezer mas megoldas van mar. Szoval ingovanyos terulet, csinald ahogy jonak latod :)

A clusterek masik fajtaja a szamitasi cluster, ezt nem a magunkfajta hegesztomunkas hasznalja hanem a muveltebb emberek. Fizikusok, biologusok, vegyeszek, ilyesmi, ezen a teruleten az MPI uralkodik meg mindig.


