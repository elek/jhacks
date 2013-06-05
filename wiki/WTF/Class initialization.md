---
creationDate: 1112707896657 
author: kocka 
contentAuthor: kocka 
title: WTF/Class initialization 
contentUpdateDate: 1112707896657 
name: WTFClass initialization 
layout: wiki 
date: 1112707896657 
creator: kocka 
---
Egy szep dolgot szeretnek bemutatni nektek, nagyon hasznos tud lenni pl [JNI](../JNI.html) eseten :D

Egy kivallo megoldas arra hogy a hiba ne ott jelentkezzen ahol kepzodik hanem par kilometerrel arreb, mint amikor ciant ontessz egy folyoba ami atfolyik egy masik orszagba. (honnan veszek ilyen peldakat?!?!)

{% highlight java %}

public class JajjAnyam \{
  private static Throwable hoppa = null;
  public JajjAnyam()\{
    if(hoppa != null)
      throw new RuntimeException(hoppa.getMessage());
  \}
  static \{
    try \{
      //static initialization thingies
    \} catch (Throwable t)\{
      hoppa = t;
    \}
  \}
\}

{% endhighlight %}
