---
creationDate        : 2004-07-28 16:08:12 +0200 
author              : admin 
title               : Prevayler 
name                : Prevayler 
layout              : wiki 
path                : Prevayler 
date                : 2006-03-26 01:42:51 +0100 
version             : 1 
creator             : kocka 
---
A Prevayler (http://www.prevayler.org/wiki.jsp) meglehetosen elter a 'szokasos' perzisztencia retegektol. O ugyanis nem hasznal semmilyen RBDMS-t. Igazabol semmit nem hasznal.
Az egesz kutyu mindossze egy par szaz(!) soros kod. A felfogasa az, hogy a memoria az szinte ingyen van, ugyhogy taroljunk mindent benne. Meghozza hagyomanyos Java objektumok formajaban. A rendszerunkkel kapcsolatos megkotesek a kovetkezoek: 

*   minden objektumunk szerializalhato kell hogy legyen. 
*   az 'adatbazison' vegzett muveletek szinten szerializalhatoak es determinisztikusak kellenek hogy legyenek. Ez azt jelenti, hogy adott allapoton adott muveletet lefuttatva mindig ugyanaz tortenjen. Emiatt a muvelet parameterenek kell minden olyan dolgot megadni, ami valtozhat (pl. rendszerido - ez mondjuk automatikusan parametere minden muveletnek, vagy pl. ha egy file-bol olvasunk, akkor ne a filenev legyen a parameter - hiszen a tartalma valtozhat idokozben, vagy torlodhet, stb. - hanem a file aktualis tartalma). 
*   Biztonsag: mi tortenik a szokasos becsapodo villam/felhekkelt rendszer/balfek takaritono eseteben? Na, az egesz ugy van megoldva, hogy minden muvelet vegrehajtasa elott a muveletet leszerializalja, es elmenti a tranzakcio-logban, ill. az egesz rendszert bizonyos idokozonkent (pl. minden ejfelkor) szepen leszerializalja egy fileba (snapshot). ha valamikor beall a crash, akkor szepen a legutolso snapshotbol visszaallitja az indulo 'adatbazist', majd az osszes, a snapshot ota tortent muveletet lefuttatja ujra rajta.

Egyszeru nem?

*   Elonyei: sokkal gyorsabb, mint barmelyik RDBMS, kevesebb szivas van az adatreteg korul. 
*   Hatranyai: nem SQL-alapu, ami miatt esetleg mas rendszer kapcsolasa bizony nehezkesse valik.

jo cikk a temarol: 

[http://www-106.ibm.com/developerworks/web/library/wa-objprev/index.html](http://www-106.ibm.com/developerworks/web/library/wa-objprev/index.html) 
A more up to date implementation (http://prevayler.codehaus.org/) By: Darwin 


Most akkow prevayler, vagy [prewayler](Missing.html)?
