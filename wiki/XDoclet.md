---
creationDate: 1097228595683 
author: kocka 
contentAuthor: kocka 
title: XDoclet 
contentUpdateDate: 1212755695081 
name: XDoclet 
layout: wiki 
date: 1212755695081 
creator: zsoltk 
---
Az XDoclet arról szólt, hogy [java](java.html) kommentekbe elhelyezett tagek segítségével kigenerálta a metainformációkat tartalmazó fileokat, többnyire valami [XML](XML.html)-t, például a [hibernate](Hibernate.html) hbm filejait, vagy a web.xml-t [webappok](webapp.html) esetén.

Ez a megközelítés a [java 1.5](java%201.5.html) [annotációk](annotations.html) megjelenésével háttérbe szorult. Jelenleg (2008) a [java 1.4](java%201.4.html) EOL fázisban van, a legtöbb framework lehetővé teszi [annotációk](annotations.html) használatát.

# Xdoclet 1

http://xdoclet.sourceforge.net/xdoclet/index.html

Generalizalt [JavaDoc](javadoc.html), ami mindenfele okos dologra kepes. peldanak okaert annotaciok segitsegevel lehet vele [EJB](EJB.html)-ket gyartani. Aki probalt mar [EJB](EJB.html)-t heggeszteni by hand, az tudja milyen jo dolog is ez.

Termeszetszeruelg az [ant](ant.html)-al nagyon jol egyutt mukodik es van neki egy rakat tag-je. kepes template-bol dolgozni es ha mar minden kotel szakad, irhatunk sajat  tag handlert. szoval szep, szagos, interaktiv:)

# Xdoclet 2

http://xdoclet.codehaus.org/

Na igen, kisse halovanyan valik el egymastol a ket xdoclet project, viszont nem kompatibilisek egymassal. Mielott megszivatnad magad azzal hogy xdoclet 1-gyel probalsz hasznalni [hibernate](Hibernate.html) 3-at, terj at xdoclet 2-re, sajnos a tagjeidet is at kell majd irnod.

Elsore az igazi lenyeges ujitas az hogy vegre normalis [maven](maven.html) plugin van hozzza, nincs minden xdoclet pluginhoz kulon [maven](maven.html) goal.

Lasd meg: [qdox](QDox.html)
