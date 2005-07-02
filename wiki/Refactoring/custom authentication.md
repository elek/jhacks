---
creationDate        : 2005-07-02 21:31:14 +0200 
author              : kocka 
title               : Kis torteneti attekintes 
name                : Refactoring/custom authentication 
layout              : wiki 
path                : Refactoring/custom authentication 
date                : 2005-07-02 21:37:14 +0200 
version             : 2 
creator             : kocka 
---
A regi frameworkokben nem volt arra semmi kozponti megoldas hogy ki milyen eroforrast hasznalhat, hogyan azonositsuk, stb, meg a ma hasznalatos webes programozasi nyelvek ([php](../PHP.html), [perl](../perl.html), satobbi) sem tartalmaz ra valami sok tamogatast.

Nade a [java](../java.html) [webapp](../webapp.html)ok deklarativ hozzaferes kezelest tartalmaznak, valamint a [alkalmazas szerver](../Alkalmazas%20Szerver.html) feladata a [webapp](../webapp.html)ok szamara az azonositast es a felhasznaloi role-ok ellenorzese. Ennyivel kevesebbet kell programozni, valamint egyetlen nagy vallalati azonositasi rendszerbe illesztheted a felhasznalodat. A custom dolgokat meg elvegezheted valahol a kodoban is, ha valami extrat akarsz.

# Problema

A problema ott kezdodik hogy ezt a kezdok, [php](../PHP.html) iranybol erkezok, vagy trehany dogok es mas gyanusan olcson kaphato munkaero sajna eleg gyakran nem tudja. Ez tobbyire oda vezet hogy nincs is valojaban biztonsagi ellenorzes, csak egy login screen ami mogott valojaban ellenorzes nelkul erheted el a funkcionalitast. Van olyan perverzio is hogy a sessionbe pakolt objektum letesese vagy nemletezese alapjan donti el hogy be van-e jelentkezve, ez az objektum pedig tobbnyire egy adatbazi szerver kapcsolat :) (Lasd a [JDBC](../JDBC.html) agymeneseket es a [WTF](../WTF.html)eket)

Pelda erre [SuhaiG](../suhaig.html) [WTF/JSP esettanulmany](../WTF/JSP%20esettanulmany.html)a.

# Workaround

Ilyenkor szerintem elso lepeskent becsomagolhatjuk a rendszert egy szabvanyos azonositasi megoldassal, ha valami specialis eroforras kell a sessionbe a idiota logikanak, akkor azt tegyuk meg a sessionlistenerrel. Majd kesobb kinyirjuk azt is :) Innentol a biztonsag legalabb elerheto, de alaposan vegig kell ellenorizni utanna a rendszert, mert tobbnyire az ilyeneket a sajat hibaik tartjak eletben.

Lasd meg: [wtf](../WTF.html), [refactoring](../Refactoring.html), [webapp](../webapp.html), [security](../security.html), [jaas](../JAAS.html) meg amit akarsz.

Naplementekor kelet fele fordulok. Arra van India. Csunyakat gondolok kozben.
