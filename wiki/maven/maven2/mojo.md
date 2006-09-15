---
creationDate        : 2006-09-15 12:01:52 +0200 
author              : kocka 
title               : maven/maven2/mojo 
name                : maven/maven2/mojo 
layout              : wiki 
path                : maven/maven2/mojo 
date                : 2006-09-15 12:01:52 +0200 
version             : 1 
creator             : kocka 
---
A mojo a [maven/maven2](../../maven/maven2.html) [plug-in](../../Missing.html) apija, kicsit [IOC](../../ioc.html) jellegu, a beallitasokat siman besetteli neked a bean-edbe, de azert nyilvan van benne valami.

Egy ilyen plugin projectet elkezdeni egyebkent nagyon konnyu. Kb ennyi:
```
mvn archetype:create -DarchetypeArtifactId=maven-plugin-archetype -DartifactId=ize-plugin -DgroupId=hu.ize
```

Esetleg megy egy 'mvn eclipse:eclipse' es [eclipse](../../Eclipse.html)-be is importalhatod a cuccot. Vegulis van olyan egyszeru mint egy [ant](../../ant.html) taszkot irni :)
