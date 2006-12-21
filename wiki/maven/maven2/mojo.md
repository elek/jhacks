---
creationDate        : 2006-09-15 12:01:52 +0200 
author              : kocka 
title               : maven/maven2/mojo 
name                : maven/maven2/mojo 
layout              : wiki 
path                : maven/maven2/mojo 
date                : 2006-12-21 10:26:49 +0100 
version             : 5 
creator             : kocka 
---
A mojo a [maven/maven2](../../maven/maven2.html) [plugin](../../plugin.html) apija, kicsit [IOC](../../ioc.html) jellegu es [pojo](../../pojo.html) alapu, innen a nev, a beallitasokat siman besetteli neked a bean-edbe, de azert nyilvan van benne valami.

Egy ilyen plugin projectet elkezdeni egyebkent nagyon konnyu. Kb ennyi:
```
mvn archetype:create -DarchetypeArtifactId=maven-plugin-archetype -DartifactId=ize-plugin -DgroupId=hu.ize
```

Esetleg megy egy 'mvn eclipse:eclipse' es [eclipse](../../Eclipse.html)-be is importalhatod a cuccot. Vegulis van olyan egyszeru mint egy [ant](../../ant.html) taszkot irni :)

Linkek:

*   [Mojo Developer Cookbook](http://docs.codehaus.org/display/MAVENUSER/Mojo+Developer+Cookbook)

Maganvelemeny ([kocka](../../kocka.html)): Imadnivalo kis cucc az egesz, frankon ki van talalva, de dokumentacio irassal nem szoszoltek a sracok :(


