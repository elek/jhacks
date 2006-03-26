---
creationDate        : 2005-04-05 15:31:36 +0200 
author              : admin 
title               : WTF/Class initialization 
name                : WTF/Class initialization 
layout              : wiki 
path                : WTF/Class initialization 
date                : 2006-03-26 01:43:01 +0100 
version             : 1 
creator             : kocka 
---
Egy szep dolgot szeretnek bemutatni nektek, nagyon hasznos tud lenni pl [JNI](../JNI.html) eseten :D

Egy kivallo megoldas arra hogy a hiba ne ott jelentkezzen ahol kepzodik hanem par kilometerrel arreb, mint amikor ciant ontessz egy folyoba ami atfolyik egy masik orszagba. (honnan veszek ilyen peldakat?!?!)

```

public class JajjAnyam {
  private static Throwable hoppa = null;
  public JajjAnyam(){
    if(hoppa != null)
      throw new RuntimeException(hoppa.getMessage());
  }
  static {
    try {
      //static initialization thingies
    } catch (Throwable t){
      hoppa = t;
    }
  }
}

```
