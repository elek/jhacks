---
creationDate        : 2006-10-01 10:53:57 +0200 
author              : kocka 
title               : JPA 
name                : JPA 
layout              : wiki 
path                : JPA 
date                : 2007-11-11 18:58:55 +0100 
version             : 2 
creator             : karenin 
---
Az [ejb 3](Missing.html)-al bevezetett új szabványos api. Legegyszerűbb taláb a [JDBC](JDBC.html)-hez hasonlítani: Van egy független interface rendszer és az alá implementálhatnak megoldásokat a szállítók. A [Hibernate](Hibernate.html) pl. gőzerővel dolgozik a Hibernate Entity Manager-en, amit lehet használni EJB3-ak alatti perzisztencia megvalósítására. De a Sunos cuccokat általában az Oracle Toplink Essential-al szállítják. A szép az, hogy ezeket bármikor lehet cserélgetni az alkalmazás alatt.

(Ja és az egész JPA-t lehet használni standalon alkalmazáskbans is)

Kb így néz ki:

```

EntityManagerFactory emf = Persistence.createEntityManagerFactory("HibernatePU");
EntityManager em = emf.createEntityManager();
SampleEntity entity = em.find(SampleEntity.class,1l);
em.close();
```

(A HibernatePU-t egy persistence.xml-ben kell definiálni, ahol megmondjuk, hogy melyik gyártó megoldását akarjuk használni.)

# JPA implementációk:


*   Hibernate
*   Toplink
*   OpenJPA
