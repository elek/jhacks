---
creationDate        : 2005-01-19 21:53:57 +0100 
author              : admin 
title               : TomcatAuthWiaPostgreSQL 
name                : TomcatAuthWiaPostgreSQL 
layout              : wiki 
path                : TomcatAuthWiaPostgreSQL 
date                : 2006-03-26 01:42:59 +0100 
version             : 1 
creator             : kocka 
---
[Receptklub](Missing.html) :)

Szoval nemreg, amikor a kis kihagyasok voltak a szerveren, a kihagyasok oka egy j2ee azonositasi schema bevezetese volt. Megosztanam a szaftosabb darabokat belole, hatha nem unjatok szet az agyatokat rajta.

Hozzavalok: 

*   [PostgreSQL](PostgreSQL.html) 7.4
*   [Tomcat](tomcat.html) 5.0 (hat senki nem futtat [EJB](EJB.html)t, minek akkor jboss... )
*   Egy szerver, vagy ketto, esetleg megegy de az mar nem tudom minek.
*   So, bors, olommentes paprika...

A problema: A Tomcat adminisztracios [webapp](webapp.html) eleg gyengecske, es arra specializalodott, hogy eroforrasokat ki tudjak osztani futasidoben. A felhasznalo management spec jobb lenne rajta kivul.

A lepesek:

Mar regebben lehetove tettem a felhasznaloknak hogy IDENT azonositassal jelentkezzenek be az adatbazisba shellbol. Igy a [Operacios rendszer](Operacios%20rendszer.html) azonositast elfogadja a [PostgreSQL](PostgreSQL.html). [howto](http://www.postgresql.org/docs/7.4/static/client-authentication.html)

Letrehoztam egy [rdbms](RDBMS.html) [schema](Missing.html)t ahol eltaroltam azokat a tablakat amik a jelszavakat es szerepkoroket tartalmazzak.

A [tomcat](tomcat.html)-ban a conf/server.xml-ben modositottam a UserDatabase elementet, most mar egy DataSourceRealm-ot hasznal. [howto](http://jakarta.apache.org/tomcat/tomcat-5.0-doc/realm-howto.html)

Na most jon a hack ( vagy [tak](tak.html) :D )

Minden juzernek kepesnek kell lennie arra hogy modositsa a sajat jelszavat, de nem lathatja semmikeppen sem senki maset. A users tablarol tuntessunk el a jogosultsagaikat, es egy stored procedure-n keresztul hagyjuk hogy updateljenek. Ez igy nez ki kb:
```
create or replace function update_my_pwd(varchar) returns void as 
'
update users set password = $1 where name = session_user
' language sql security definer;
```

Innentol kezdve tok ecceru olyan scripteket irni, amikkel biztonsagosan kezelni lehet a jelszavakat, role-okat, satobbi.

Sok borssal fuszerezve talaljuk.

UDFekbol nagyon sokmindent lehet fozni, jo alapanyag.
