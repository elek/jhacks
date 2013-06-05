---
creationDate: 1120123144831 
author: suhaig 
contentAuthor: suhaig 
title: WTF/JSP esettanulmany 
contentUpdateDate: 1120123144831 
name: WTFJSP esettanulmany 
layout: wiki 
date: 1120123144831 
creator: suhaig 
---
Sajnaljatok egy kicsit legyetek szivesek. Koszi :)

Egy webes alkalmazasrol lenne szo, nem egy nagy durranas, semmi extra.<br/>Index.jsp-vel indul a flow, az oldal azonnal felhasznaloi nevet es jelszot ker, szoval ez lenne a loginform, ha a szerzo tudta volna, hogy mi az. A form-ot a Login.jsp dolgozza fel, annyi konnyites van, hogy legalabb egy bean-en keresztul fordul az adatbazishoz, hogy ellenorizze a jelszot. Igen a jelszot, mert ha a felhasznaloi nevet nem talalja az adatbazisban, akkor ArrayIndexOutOfBoundsException-nel elszall, mert arra szamit, hogy a SELECT mindig ad neki vissza valamit. Ha nem jo a jelszo, akkor a Login.jsp-bol van egy sendRedirect hivas a Feedback.jsp-re. Persze elotte egy-ket dolgot meg kiir a response stream-be, tehat IllegalStateException-nel elhal az egesz.<br/> De tegyuk fel, hogy nem hal el es menjunk tovabb, mert az igazi szepsegek csak most jonnek.<br/>
Minden jsp, igy a Feedback.jsp is ugy indul, hogy include-olja az Authentication.jsp-t. Ez annyit csinal, hogy megnezi, hogy be van-e jelentkezve a felhasznalo. Ha nincs, akkor ismet csak egy sendRedirect hivason keresztul tovabbit az ErrorMessage.jsp-re. Persze itt is IllegalStateException van. Leesett?<br/>
Ha valakinek nem lenne tiszta: nem tudjuk megmondani a felhasznalonak, hogy rossz jelszot adott meg, mert nincs bejelentkezve! A sendRedirect hivas a response irasa után mar csak a desszert.<br/>
Az en feladatom az lenne, hogy uj funkciokat adjak a rendszerhez. 
