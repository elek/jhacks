---
creationDate        : 2004-08-05 10:40:57 +0200 
author              : admin 
title               : ant 
name                : ant 
layout              : wiki 
path                : ant 
date                : 2006-03-26 01:43:05 +0100 
version             : 1 
creator             : kocka 
---
![image](http://hackers.forgeahead.hu/space/banners/sidebar/ant_logo_large.gif)<br/>
__ANT__

[http://ant.apache.org/](http://ant.apache.org/)

Napjaink legszelesebb korben elfogadott [build](build.html) toolja elsosorban [java](java.html) fejlesztesekhez.

Az anthoz erdemes ismerni a tortenelmi hatteret: a [unix](unix.html) make parancsot. A make parancsot foleg [C](C.html)/C++ projectekben hasznaljak arra hogy a forditasi folyamatot automatizaljak es fel is gyorsitsak azaltal hogy csak a szukseges parancsokat hajtjak vegre. A make-nek megmondod hogy milyen file-okat kell elkeszitenie, es melyik file mibol keszul el es hogyan. A make kezeli a file-ok fuggosegeit, es ha egy file foggosegei kozul valami ujabb mint maga a file, akkor azt a file-t ujraforditja. Pl:
```
all: sayhello

sayhello: sayhello.o hellolib.o

```

Az ant :

*   a build fileok [XML](XML.html) fileok, amivel kicsit konnyebben atlatja es megerti az is aki nem boklaszik ant fileokban egesz nap
*   szakit a file alapokkal
*   vegre platformfuggetlen (ha nem irsz baromsagot a build file-ba ugye ;) )
*   kihasznalja a java nyelv minden lehetoseget, peldaul a szabvanyos [JDBC](JDBC.html) api-t is

A build file egy projectet tartalmaz, ami tartalmazza a taskokat es az egyeb globalis strukturakat (tulajdonsagok, utmegadasok, stb). Az tartgetek mindenfele taskokat tartalmazhatnak. A tasokok gyakorlatilag a proceduralis leirasa annak hogy mit kell tenni. A targetek kozott termeszetesen lehetnek fuggosegek, a korfuggosegeket az ant detektalja es megbunteti :)

pl:
```
<?xml version="1.0"?>

<project name="igazsagosztas" default="all">

  <target name="greeting" description="says hello nice">
     <echo>Ho:jj! Hello!</echo>
  </target>

  <target name="all" depends="greeting">
     <echo>es kesz is...</echo>
  </target>

</project>
```

A legfontosabb build taskok megvannak alapbol, ha valami esetleg hianyozna akkor az architektura kiegeszithato mas taskokkal, amit a neten beszerezhetsz, vagy irhatsz ha nagyon perverz vagy.

linkek:

*   oreg mainstream technologia leven mindenhol tele van vele minden, nezd meg a sidebaron :)

Alternativa lehet esetleg a [maven](maven.html)

Az Ant a [Netbeans](Netbeans.html) 4.x-es szeria beepitett build rendszere lesz, ami garantalja azt hogy a [Netbeans](Netbeans.html)re epitett projectek barmilyen kornyezetben konnyen lefordithatoak. Termeszetesen szinte minden [IDE](IDE.html) integralta es valamilyen feluletet biztosit hozza.
