---
creationDate: 1108550508146 
author: kocka 
contentAuthor: kocka 
title: call handler module 
contentUpdateDate: 1108550508146 
name: PL-Jcall handler module 
layout: wiki 
date: 1108550508146 
creator: kocka 
---
A call handler module egy C nyelven irt funkcio [PostgreSQL](PostgreSQL.html) 8.0-hoz es 7.4-hez, ami egy par egyeb modult is magabafoglal.

Egy Pl-J eljaras meghivasakor a call handler module kapja meg a vezerlest. A hivasi informaciobol letrehozza a hivasi infot, elkuldi a java szervernek, es kiszolgalja a java szerver tovabbi kereseit ([logging](Logging.html), [jdbc](JDBC.html) hivasok).

Ket helyettesitheto almodult tartalmaz:

*   callmaker: ez gyakorlatilag csak a szabadon szoveges formatumban leirt funkciobol kovetkezteti ki a osztaly es metodis nevet es egy-ket egyeb infot.
*   config: a modulok es a call handler ehhez fordul minden konfiguracios informacioert. A jelenleg egyetlen implementacio mindent db tablaban tart.
