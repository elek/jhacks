---
creationDate        : 2005-01-16 21:04:55 +0100 
author              : admin 
title               : beanutils 
name                : beanutils 
layout              : wiki 
path                : beanutils 
date                : 2006-03-26 01:43:07 +0100 
version             : 1 
creator             : kocka 
---
__Commons BeanUtils__

[http://jakarta.apache.org/commons/beanutils/](http://jakarta.apache.org/commons/beanutils/)

Egy [commons](commons.html) subproject amire valoszinuleg ugy is egyszer szukseged lesz :)

Tegyuk fel hogy az alkalmazaslogikad kap beaneket, es te konkretan nem tudod hogy mifele beanek lesznek, mert lehet akarmi is, de be kell allitanod rajta tulajdonsagokat vagy ki kell olvasni oket. Nagy valoszinuseggel nem tudod elore a tulajdonsag neveket sem, mert az nem lenne poen.

Na nezzuk csak hogy is irjuk a tulajdonsagot:
```
BeanUtils.setProperty(obj, propName, value);
```

Es visszaolvasni
```
PropertyUtils.getProperty(obj, propName);
```

Hat kb ennyi, nem erdemes a tanulmanyozasara szanni 2 percnel tobbet, nem erdemes 1-2 orat pocsolni azon hogy sajat utilt irjal ugyanerre, es plane nem erdemes napokkal vagy hetekkel meghosszabbitani egy projectet tobb tonnanyi manualis [reflection](reflection.html) programozas kedveert.
