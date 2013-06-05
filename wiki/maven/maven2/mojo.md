---
creationDate: 1158314512242 
author: kocka 
contentAuthor: kocka 
title: maven/maven2/mojo 
contentUpdateDate: 1166693209968 
name: mavenmaven2mojo 
layout: wiki 
date: 1166693209968 
creator: kocka 
---
A mojo a [maven/maven2](../../maven/maven2.html) [plugin](../../plugin.html) apija, kicsit [IOC](../../ioc.html) jellegu es [pojo](../../pojo.html) alapu, innen a nev, a beallitasokat siman besetteli neked a bean-edbe, de azert nyilvan van benne valami.

Egy ilyen plugin projectet elkezdeni egyebkent nagyon konnyu. Kb ennyi:
{% highlight java %}
mvn archetype:create -DarchetypeArtifactId=maven-plugin-archetype -DartifactId=ize-plugin -DgroupId=hu.ize
{% endhighlight %}

Esetleg megy egy 'mvn eclipse:eclipse' es [eclipse](../../Eclipse.html)-be is importalhatod a cuccot. Vegulis van olyan egyszeru mint egy [ant](../../ant.html) taszkot irni :)

Linkek:

*   [Mojo Developer Cookbook](http://docs.codehaus.org/display/MAVENUSER/Mojo+Developer+Cookbook)



Maganvelemeny ([kocka](../../kocka.html)): Imadnivalo kis cucc az egesz, frankon ki van talalva, de dokumentacio irassal nem szoszoltek a sracok :(




