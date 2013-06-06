---
creationDate        : 2004-07-27 10:41:28 +0200 
author              : kocka 
title               : servlet_jsp 
name                : servlet_jsp 
layout              : wiki 
path                : servlet_jsp 
date                : 2007-10-25 17:22:51 +0200 
version             : 4 
creator             : kocka 
---
Servlet + JSP a legegyszerubb megoldas valamifele [MVC](MVC.html) architektura kialakitasara a webalkalmazasban.

Minden felhasznalio interakcional a szervlet kapja meg a vezerlest, kibutykoli a requestbol hogy milyen parameterekkel kell futnia, aztan bean-eket hoz letre, azokat atadja a jsp-nek, es a jsp pedig megjeleniti.<br/>
Tehat M=beans, V=[jsp](JSP.html), C=[servlet](servlet.html).

Igazabol nagyon faj tucat szervletet irni, es mindet a web.xml-be regisztralni, ezert tobbnyire oda jutottak a nepek, hogy csak egy servletet irnak, es az dispatcheli a requesteket az action-ok kozott. Na ez mar igy kozel all a [struts](struts.html)-hoz, csak meg hianyzik belole jopar dolog.

Ja itt egy jo konyv hozza:
[http://www.theserverside.com/books/addisonwesley/ServletsJSP/index.tss](http://www.theserverside.com/books/addisonwesley/ServletsJSP/index.tss)
