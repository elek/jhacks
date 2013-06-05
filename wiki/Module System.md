---
creationDate: 1180728560718 
author: karenin 
contentAuthor: karenin 
title: Module System 
contentUpdateDate: 1180728560718 
name: Module System 
layout: wiki 
date: 1180728560718 
creator: karenin 
---
Jobb híján lett ez a neve a snipnek. Alapvetően a moduláris tervezés megvalósításrairól van szó. 

Általános jellemző:

# vannak modulok (csomagok)


# van valamilyen leíró


# a leíróban név és verzió van definiálva


# a leíró ezek alapján dependecyket definiál


# a leíró sokszor definiálja a publikus és privát részeket


# a modulok sokszor repositorykban vannak tárolva

A legizgalmasabb számomra pl. publikus és privát osztályok/csomagok megadása. Az azért frankó, mert ekkor lehetséges az, hogy ha két modul is monduk egy XMLparser termélktől függ, de két verziótól, akkor nem akadnak össze, mert a modulokból csak a publikus csomagokat látja a felhasználó.

Lásd még:
* [OSGi](OSGi.html)
* [JSR-277](JSR-277.html)
