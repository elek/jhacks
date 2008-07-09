---
creationDate        : 2006-10-01 10:53:57 +0200 
author              : kocka 
title               : JPA 
name                : JPA 
layout              : wiki 
path                : JPA 
date                : 2008-07-10 00:30:19 +0200 
version             : 10 
creator             : karenin 
---
Az [ejb3](EJB3.html)-al bevezetett új szabványos [persistence](persistence.html) api. Legegyszerűbb taláb a [JDBC](JDBC.html)-hez hasonlítani: Van egy független interface rendszer és az alá implementálhatnak megoldásokat a szállítók. A [Hibernate](Hibernate.html) pl. gőzerővel dolgozik a Hibernate Entity Manager-en, amit lehet használni EJB3-ak alatti perzisztencia megvalósítására. De a Sunos cuccokat általában az Oracle Toplink Essential-al szállítják. A szép az, hogy ezeket bármikor lehet cserélgetni az alkalmazás alatt.

(Ja és az egész JPA-t lehet használni standalon alkalmazáskbans is)

Kb így néz ki:

```

EntityManagerFactory emf = Persistence.createEntityManagerFactory("HibernatePU");
EntityManager em = emf.createEntityManager();
SampleEntity entity = em.find(SampleEntity.class,1l);
em.close();
```

(A HibernatePU-t egy persistence.xml-ben kell definiálni, ahol megmondjuk, hogy melyik gyártó megoldását akarjuk használni.)

__[IDE](IDE.html) támogatás__:

*   [Eclipse](Eclipse.html) [Dali](http://www.eclipse.org/webtools/dali/main.php)


__JPA implementációk__:

*   [Hibernate](Hibernate.html)
*   [Toplink](Toplink.html)
*   [OpenJPA](OpenJPA.html)
*   [cayenne](Missing.html) (folyamatban)
*   Kodo
*   [eclipselink](eclipselink.html)

Cikkek, prezentációk:

*   [Java Persistence 2.0](http://www.parleys.com/display/PARLEYS/Java+Persistence+2.0?showComments=true)
*   [Advanced Topics in JPA](http://www.parleys.com/display/PARLEYS/Advanced+Topics+in+JPA)
