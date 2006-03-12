---
creationDate        : 2006-03-12 14:25:40 +0100 
author              : pedro 
title               : REST 
name                : REST 
layout              : wiki 
path                : REST 
date                : 2006-03-12 16:26:47 +0100 
version             : 5 
creator             : kocka 
---
Egy Roy T. Fielding nevű ember megunta az ostoba módot, ahogyan a .com lufi idején kinézett az Internet (most sem jobb a helyzet) és a filozófia disszerzációjában leírt valamit, ami azóta híres lett:

[Representational State Transfer](http://en.wikipedia.org/wiki/Representational_State_Transfer)

A lényege röviden:

*   minden erőforrás: az "információ" valamilyen "reprezentációja" (kicsit ködös, de érthető:)
*   a [HTTP](HTTP.html) GET, POST, PUT, DELETE, stb utasításait használjuk arra amire kell
*   az [URI](URI.html)-k tükrözzenek némi szemantikát,
*   állapotmentes kliens-szerver felépítés, azaz a kéréseknek mindig magukban kell hordozni az összes információt, amivel őket teljesíteni lehet és:
*   a belső állapotátmenetek rejtve maradjanak a kérő elől.

Szakít a [SOAP](SOAP.html) szemléletű [RPC](RPC.html) webszolgáltatás világgal.

Pl:
A [http://pedro.hu/index?getUser=pedro](http://pedro.hu/index?getUser=pedro) kérés helyett a [http://pedro.hu/user/pedro](http://pedro.hu/user/pedro) a "szemantikusabb". Aztán a kiszolgáloó lehet, hogy egy index?getUser=pedro műveletet fog végezni, de ez az átmenet számomra láthatatlan. Ha törölni akarom a pedro erőforrást, akkor a [http://pedro.hu/user/pedro](http://pedro.hu/user/pedro) [URI](URI.html)-t DELETE [HTTP](HTTP.html) kéréssel bököm meg ahelyett, hogy [http://pedro.hu/index?getUser=pedro&operation=delete](http://pedro.hu/index?getUser=pedro&operation=delete) vagy [http://pedro.hu/index?deleteUser=pedro](http://pedro.hu/index?deleteUser=pedro) GET kéréseket használnék ... stb.

2006-ban jobb a helyzet, mint 2000 környékén, az előző példa egységes környezetben megvalósítható, általános megoldása: [http://pedro.hu/user/pedro?operation=delete](http://pedro.hu/user/pedro?operation=delete) . Nos ... félsiker:) De a haladás érezhető:)

Vannak jó kezdeményezések. A [Sun](Sun.html) féle [JEE](JEE.html) elképzelés (sajnos nem az ...) web konténerei szabvány szerint erre pillanatnyilag alkalmatlanok, mivel azok [SOAP](SOAP.html) webszolgáltatásokra vannak felkészítve. Az [JEE](JEE.html) 1.5-ös változata viszont már lehetőséget bíztosít erre. Én a [GlassFish](glassfish.html)-sel próbálkoztam és tényleg lehet:)

Ami szabványos és jelenleg is képes ilyen [URI](URI.html) kezelésre az a [Jetty](jetty.html). Erre alapozva készült is egy framework:

[RESTlet](http://www.restlet.org/)

Nem tudom érdemes-e használni. Úgy is jön az 1.5-ös [JEE](JEE.html).

([Pedro](pedro.html) irasai nyoman :) ) (valóban ezt is én írtam, de mivel itt [is](URI.html) elbénáztam [kocka](kocka.html)-nak ki kellett ismét segítenie ... többé nem fordul elő ... úttörő becsszó:)
