---
creationDate        : 2004-07-26 12:02:22 +0200 
author              : kocka 
title               : Eclipse 
name                : Eclipse 
layout              : wiki 
path                : Eclipse 
date                : 2006-12-26 22:49:59 +0100 
version             : 15 
creator             : zsoltk 
---
Hat akkor aljon is itt nemi bemutato a prg-rol.


-   [eclipselink](eclipselink.html)



# Bemutato

Bar a neve azt jelenti, hogy napfogyatkozas, ami ugye sotetseggel jar egyutt, megis azt kell mondjam, hogy az egyik legjobban hasznalhato [IDE](IDE.html)-rol beszelunk. Fontos azonban megjegyezni, hogy jelen esetben ez egy 2 oldalu dolog.

Magaban az Eclipse csomagban nem igazan van sok minden, amit hasznalni lehetne. Marmint kulonbozo libekre, kornyezetekre gondolok. Ilyen szempontbol egy [Oracle](Oracle.html) [JDeveloper](JDeveloper.html), egy [Borland](borland.html) [JBuilder](JBuilder.html), vagy egy [Sun](Sun.html) [NetBeans](Netbeans.html) sokkal tobbet tud. Tehat ilyen szempontbol egy Eclipse meglehetosen fapados valami. De! Halistennek a [eclipse/plug-in](Eclipse/Plug-in.html) felfogasa annyira egyszeru es szep, hogy rengeteg letoltheto beepulo van a neten. Ha ezt szamba vesszeuk, akkor egyertelmuen kiejelenthetjuk, hogy a leheto legsokretubb [IDE](IDE.html)-rol beszelunk. Ha ehhez meg hozzaveszuk a hasznalhatosagot... Szoval nem veletlen, hogy ennyien szeretik.

Peldanak okaert az [IBM](IBM.html) Application Developer-e is erre a platformra epul. Aki ismeri annak nem kell magyaraznom. Aki nem annak elegyen eleg annyi, hogy annyire sokretu funkcionalitast mint a WSAD szvsz egyik IDE sem kinal.

# Install

Mivel [Java](java.html) alapu [IDE](IDE.html)-rol beszelunk, ezert barmilyen platformon hasznalhato, ahol van VM. Elvileg, mert egy sajat megjelenitesi konyvtarat hasznal. Ez pedig az [SWT](swt.html) (Simple Windowing Toolkit). Szebb, gyorsabb, kevesbe eroforrasigenyes, es kell hozza nativ binaris. Szoval csak azon lehet futtatni, ahol van ilyen. Ezek a platformok pedig a kovetkezoek:

*   [Linux](Linux.html)
*   [Windows](Windows.html)
*   [Solaris](Solaris.html)
*   AIX
*   HP-UX
*   Mac OS

Ez altalaban eleg szokott lenni, de letoltheto a forras is, ha mondjuk valaki Amigara vagy ZX spectrumra szeretne forditani...

De hagyjuk a hulyeseget:-)

Az Eclipse-et ketfelekeppe lehet installalni. Vagy a platform SDK-t tolti le az ember, vagy a kulonbozo reszekbol rakja ossze.

Erdemes altalaban a Platform SDK-t letolteni, mivel meretre nagyjabol ugyanannyit kell tolteni, ha egy hasznalhato Eclipse-t szeretnel...

De ha megis a masodik modszert valasztod, akkor a szukseges csomagok leirasa kovetkezik:

*   Plaform Runtime Binary: ez mindenfelekeppen kell, ez az alap.
*   JDT Runtime: Java development tools. Ez ahhoz kell, hogy Javaban tudjal valamit fejleszetni. (A PRB semmit nem tartalmaz amivel fejleszteni lehetne...)

Na most ez igy nem olyan sok, de altalaban az a vege, hogy az ember televagja [eclipse/plug-in](Eclipse/Plug-in.html)-ekkel, amik viszont mindenfele dolgokat igenyelnek. Azokat meg persze le kell tolteni. Szoval erdemes a Platform SDK-t lehuzni. (-> lasd: [callisto](Callisto.html))

Szoval a dolog gyakorlatilag abbol all, hogy a megfelelo platformra le kell toltenunk biz. fajlokat.

Amit erdemes meg tudni: A jelenleg letoltheto verziok a 3.0 es a 2.1.3. Gyakorlatilag mind a ketto stabil. Termeszetszeruleg a 2.1.3 a regebbi. Semmi gond nincs vele, bar a funkcionalitasa a 3.0-nak lenyegesen nagyobb. Amiert erdemes lehetletolteni, az az mert biz. plug-inek meg mindig csak 2.1.3 ala vannak meg. De idovel majd ez is valtozik.

Megjegyeznem meg, hogy a [Linux](Linux.html)os verziobol erdemes a GTK frontendet valasztani, bar van aki a Motifra eskuszik.

# [Plugin](plugin.html)ek

Ez az a dolog, amiben az Eclipse rettenetesen eros. Annyit es olyat tudsz tolteni, amit csak nem szegyelsz. Gyakorlatilag maga a [Java](java.html) [IDE](IDE.html) is egy plugin. Csak eppen ez a fo plugin, amikre aztan szepen ra leehet tolni a tobbieket. 

Mivel alapbol az IDE-sok mindent nem lehet csinalni, ezert erdemes hozza plugineket toltogetni. Hogy alapbol mit tud az IDE? Java editalas, Ant build kezeles, Debug, CVS. Nagyjabol. Latszik szepen, hogy nem valami nagy funkcionalitas...

Ha pluginek kellenek, akkor ezeket megtalalalod a [Eclipse/Plug-in](Eclipse/Plug-in.html)-s reszben.

Amit persze kihagytam, az a site ahonnan letoltheted az egeszet: [http://www.eclipse.org](http://www.eclipse.org)

# Problemak

Hiaba jo a plugin rendszer, akkor is magadnak kell keresgetni a pluginokat, amibol konnyen kerekedhet egy hatalmas kaosz.<br/>
Nagy meretu projectek (mondjuk 20 mega felett) eseteben az Eclipse bosszantoan lassu tud lenni, jobb ha kikapcsolod az automatikus forditast...

# Eclipse leszarmazottak

*   [websphere app dev](Websphere%20App%20Dev.html) ([IBM](IBM.html))
*   [myeclipse](myeclipse.html)
*   [weblogic workshop](weblogic%20workshop.html) ([BEA](bea.html)) a 9-estol kezdve, a 8.x-es szeria sajat volt

# Linkek

*   [http://eclipse-wiki.info/](http://eclipse-wiki.info/) Mint a neve is mutatja, egy wiki eclipse temakorben
*   [http://planeteclipse.org/planet/](http://planeteclipse.org/planet/) eclipse planet 
*   [Az eclipse debug csapat blogja](http://eclipse-debug.blogspot.com/)


