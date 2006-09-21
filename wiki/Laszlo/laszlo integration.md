---
creationDate        : 2006-09-21 11:49:32 +0200 
author              : kocka 
title               : Laszlo/laszlo integration 
name                : Laszlo/laszlo integration 
layout              : wiki 
path                : Laszlo/laszlo integration 
date                : 2006-09-21 11:49:32 +0200 
version             : 1 
creator             : kocka 
---
A laszlo a [webservices](../WebServices.html), [soap](../SOAP.html), [xml-rpc](../xml-rpc.html) es mas [rpc](../RPC.html) hivasain segitsegevel konnyen integralhato meglevo es futo rendszerekhez. Ez persze csak proxy-s felallasban mukodik, amivel kapcsolatban azt kell tudni hogy a hivas _nyilvan_ nem a browserbol fog kiindulni, hanem a browser elkuldi a kerest a szervernek aki majd vegrehajtja az [rpc](../RPC.html) hivast.

Ez tobbnyire eleg, de azert nem mindig elfogadhato megoldas az hogy meg egy halozati hivast betegyunk, meg egy webappot deployoljunk, ez kisse pazarlos megoldas. Meg tehetjuk viszont azt hogy a mar letezo alkalmazasunkat epitjuk be a [laszlo](../Laszlo.html) appba, es siman javarpc segitsegevel hasznaljuk.

Peldaul ha a [spring](../spring.html)es beanjeinket akarjuk elerni, akkor irhatunk egy listenert, ami bedobalja a [laszlo](../Laszlo.html) "__lzobj" map-jebe a [spring](../spring.html) context objektumait. Eleg egyszeru iteracio, ezek utan a spring beanek hivhatoak javarpc-n keresztul, de ez tetszoleges mas [ioc](../ioc.html) kontenerrel megoldhato.
