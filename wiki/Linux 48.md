---
creationDate        : 2006-11-13 11:29:33 +0100 
author              : kocka 
title               : Linux 48 
name                : Linux 48 
layout              : wiki 
path                : Linux 48 
date                : 2006-11-22 13:09:08 +0100 
version             : 6 
creator             : kocka 
---
Na ide kaptok egy beszamolot az esemenyrol. :)

Yikulju Ribus ([Elte](elte.html)) csapat:

*   Kelmen Viktor
*   Nemet Zsolt Balazs
*   rosszmagam ([kocka](kocka.html))

15 csapat nevezett iden, 2 nem tudott eljonni, 2 feladta

[IBM](IBM.html) [Linux](Linux.html) 48 - [java](java.html) programozoi bajnoksag felsooktatasi hallgatoknak

Pentek kora delutan, az [IBM](IBM.html) infoparkbeli epuleteben gyuleketek a versenyzok es a szervezok. Rovid es hatekony megnyito utan a [BME](Missing.html) V2 epuletebe sereglettunk at, ahol kiosztottak az eroforrasokat es a feladatokat.

A feladat kb ez: Irjatok egy automagikus ugyfel support webalkalmazast. A ugyfel kerdeseket tesz fel interaktivan, amire a szerver automatikaja valaszol. Az adminisztracios feluleten az adminisztrator be tudjon kapcsolodni a parbeszedbe, ha a szerver nagy hulyesegeket mond. Szoval [AI](AI.html) jellegu feladat.

Eszkozok elore installalva:

*   [db2](DB2.html)
*   [websphere app dev](Websphere%20App%20Dev.html), bele integralt [websphere](Websphere.html) [alkalmazas szerver](Alkalmazas%20Szerver.html)rel, sajna csak beleintegralva hasznalhato.

Eleg hamar kiderult hogy annyira nem popec az installacio, ezek ubuntu [linux](Linux.html)ok voltak, ugy latszik vannak vele bajok. Azert ez meg nem volt ok a panikra mert a kickstart projectunket ugy csinaltuk meg hogy a [maven](maven.html) kigeneralja nekunk a descriptort tobbfele [IDE](IDE.html) hez. Viszont ekkor kiderult hogy egyszeruen nincs hely a gepeken ahhoz hogy a kiarchivalt [maven](maven.html) repot feltegyem. Gyasz.

Ugyhogy gyorsan dobtuk a [maven](maven.html)t is, atnyergeltunk [eclipse](Eclipse.html)re es [myeclipse](myeclipse.html)re, amivel eleg pipecul tudott porogni a csapat.

Technologia:

*   [hibernate](Hibernate.html)
*   [struts](struts.html), mert ahhoz van ide tamogatas
*   [spring](spring.html)
*   [lucene](Lucene.html)
*   ja es [derby](Derby.html) a [db2](DB2.html) helyett
*   [ajax](ajax.html) mindenhova
*   dokumentacio: [openoffice.org](OpenOffice.org.html) es [argo uml](Argo%20UML.html)

Az ajax-tol ugy nezett ki az UI mint egy csoda, Viktor nagyon vagja az egeszet :)

A csapat igen kemenyen lenyomta az egesz fejlesztest. 48 ora alatt ugy kb 6-8 ora alvassal fejenkent, igencsak kemenyen megtoltuk. (Mondjuk en beteg voltam es idonkent szetestem, de hat van ilyen). Ugy sacc/kb par oranyi fejlesztes maradt hatra a teljes befejezesbol.

Linkek:

*   [Élménybeszámoló az IBM 48 órás programozói versenyéről](http://www.javaforum.hu/?newsId=170)
