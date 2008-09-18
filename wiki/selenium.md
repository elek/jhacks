---
creationDate        : 2006-07-27 11:24:05 +0200 
author              : kocka 
title               : selenium 
name                : selenium 
layout              : wiki 
path                : selenium 
date                : 2008-09-18 19:05:20 +0200 
version             : 9 
creator             : kocka 
---
[http://www.openqa.org/selenium](http://www.openqa.org/selenium)

Egy eszkoz [functional testing](functional%20testing.html) feladatokhoz. Van hozza egy par [plugin](plugin.html) tobb fele browserhez, peldaul [firefox](Missing.html)hoz, amivel lehet felvetelt csinalni a [webapp](webapp.html)od tesztjebol. Maga a plugin kepes kulonbozo formatumokban elmenteni a tesztleirast, peldaul [java](java.html)ban is, ami egy az egybe copy-paste utan kivalloan megfelel [junit](junit.html) tesztnek.

A junit teszthez viszont meg szukseged lesz a selenium-rc-re (remote control), ez egy kis szerverbol all, ami elinditja neked magat a browsert (ez egyebkent egy kicsit fajdalmas pontja a tesztnek) es egy http porton keresztul mondhatod neki hogy mikor mit csinaljon. O sajat magan belul javascripttel elintezi.

Hat a nyilvanvalo hatranya az az hogy ehhez pl [unix](unix.html)on egy X szervernek kell fusson (vagy valami ami annak tűnik), [windows](Windows.html)on pedig valószinűleg egy bejelentkezett felhasználóra van szükség.

A [java](java.html)s api (Selenium-RC) hozza kicsit flat, ugy 9 osztaly, parszaz metodus, a lenyeg a Selenium osztaly, ami kb ugy nez ki mint egy browser, persze csak kepletesen.

![image](http://upload.wikimedia.org/wikipedia/commons/thumb/2/2e/Se%2C34.jpg/125px-Se%2C34.jpg)<br/>
_ hat kb igy nez ki :) _


