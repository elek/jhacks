---
creationDate        : 2004-12-22 11:48:26 +0100 
author              : kocka 
title               : PL-J/ObjectStorage 
name                : PL-J/ObjectStorage 
layout              : wiki 
path                : PL-J/ObjectStorage 
date                : 2005-04-20 23:46:04 +0200 
version             : 4 
creator             : kocka 
---
A [PL-J/Devtools](../PL-J/DevTools.html) for utan az ObjectStorage otlet is kicsit kanyarodik. Egy kis kiegeszites lenne a forkolt projecten.

```

import java.util.Date;

/**
 * @plj.rdbmstype name="jPerson"
 */
public class Person {
 Date birthDate;
 String name;
 public Date getBirthDate() { return birhthDate; }
 public void setBirthDate(Date newBirthDate) { birthDate = newBirthDate; }
 public String getName() { return name; }
 public void setName(String newName) { name = newName; }
}

```

Generalt kodok:
```
create type jPerson

create function jPerson_getName(jPerson) returns varchar as 
'
class=PersonHelper
method=jPerson_getName
' language 'PL-J' immutable

-- satobbi
```

remelem az otletet ertitek.
Na most mivel a funkciok _immutable_k ezert konnyen keszithetunk rajuk indexet, azaz a sebessegbol valoszinuleg nem veszitunk valami sokat, cserebe kapunk egy erdeks cuccot.

Konkretan a pelda medint kicsit butus, de legalab ecceru.

Lasd meg: [PL-J/DevTools](../PL-J/DevTools.html)
