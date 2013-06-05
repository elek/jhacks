---
creationDate: 1128378195006 
author: kocka 
contentAuthor: kocka 
title: WTF/Rape the Oracle 
contentUpdateDate: 1128378195006 
name: WTFRape the Oracle 
layout: wiki 
date: 1128378195006 
creator: kocka 
---
Nyilvan nem a matrixban az oregmammert, hanem az [oracle](../Oracle.html) [rdbms](../RDBMS.html)t. Van ennek egy [oracle advanced queue](../oracle%20advanced%20queue.html) nevu feature mar a 8.x-es szeriatol kezdve, szoval evek ota, ez arra jo hogy PL/SQL-bol be tudj nyomni queue-nak latszo tablaba mindenfele adatot. [Xml](../XML.html)t, felhasznaloi adattipusokat, szoveget, stb.

Az [oracle](../Oracle.html) AQ nem [jms](../JMS.html) szerver abban a tekintetben hogy a kliens apija egybol az [RDBMS](../RDBMS.html)hez kapcsolodik, szoval adni kell neki egy [JDBC](../JDBC.html) kapcsolatot (tipikus oracle stilus, keptelenek szabvanyosan csinalni). Akkor viszont megis hogy a turoba fogjuk integralni egy [alkalmazas szerver](../Alkalmazas%20Szerver.html)be? Na es erre jott fel egy srac azzal hogy mivel az [Oracle](../Oracle.html) AQ osztalyainak konstruktorai mind private-ok, ezert o is ir egy oracle.jms package-t :) Igy majd belelathat. A forras fent van a [bea](../bea.html) dev2dev cuccan.

Nyilvan a [java](../java.html) nem ennyire hulye, vagy az egyik jarbol vagy a masikbol johet fel egy package, nincs am trukkozes, olyan sealing violationt fox kapni mint allat :) Egy megoldas lenne: megpatkolni vele az oracle kliens jarokat. Jehova orizz. Inkab irnek egy sajat wrappert.
