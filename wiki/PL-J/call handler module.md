---
creationDate        : 2005-02-16 11:41:48 +0100 
author              : admin 
title               : call handler module 
name                : PL-J/call handler module 
layout              : wiki 
path                : PL-J/call handler module 
date                : 2006-03-26 01:42:50 +0100 
version             : 1 
creator             : kocka 
---
A call handler module egy C nyelven irt funkcio [PostgreSQL](../PostgreSQL.html) 8.0-hoz es 7.4-hez, ami egy par egyeb modult is magabafoglal.

Egy Pl-J eljaras meghivasakor a call handler module kapja meg a vezerlest. A hivasi informaciobol letrehozza a hivasi infot, elkuldi a java szervernek, es kiszolgalja a java szerver tovabbi kereseit ([logging](../Logging.html), [jdbc](../JDBC.html) hivasok).

Ket helyettesitheto almodult tartalmaz:

*   callmaker: ez gyakorlatilag csak a szabadon szoveges formatumban leirt funkciobol kovetkezteti ki a osztaly es metodis nevet es egy-ket egyeb infot.
*   config: a modulok es a call handler ehhez fordul minden konfiguracios informacioert. A jelenleg egyetlen implementacio mindent db tablaban tart.
