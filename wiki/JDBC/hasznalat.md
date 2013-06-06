---
creationDate        : 2005-02-16 15:51:51 +0100 
author              : admin 
title               : Nehany gyakorlati tanacs 
name                : JDBC/hasznalat 
layout              : wiki 
path                : JDBC/hasznalat 
date                : 2006-03-26 01:42:42 +0100 
version             : 1 
creator             : kocka 
---
A [JDBC](../JDBC.html) szolgaltatasokat unmanaged kornyezetben ugy tudod elerni, hogy:
```
Class.forName("my.pet.database.Driver");
DriverManager.getConnection("jdbc:pet:database","kocka","kocka");
```

A [JDBC](../JDBC.html) Specifikacio szerint minden driver implementaciojanak class initializereben regisztralni kell a Driver egy peldanyat a DriverManager-ben.
Managed kornyezetben ([Alkalmazas szerver](../Alkalmazas%20Szerver.html)) ha esetleg JDBC hasznalatra vetemedsz, hasznald szepen a [JNDI](../JNDI.html)-t egy DataSource lookupolasahoz, es szerezz connection-t abbol:
```
InitialContext ctx = new InitialContext();
DataSource dsrc = (DataSource)ctx.lookup(dataSrcCtx);
Connection conn = dsrc.getConnection();
```

*   Managed kornyezetben hasznald a [JTA](../JTA.html)-t a JDBC [tranzakcio](../Missing.html)k helyett, jobb ha a [DAO](../DAO.html)-dban soha nem is probalsz commit-ot hivni.
*   Lenyeges pont az is, hogy __NE FELEJTSD EL LEZARNI AZ EROFORRASOKAT__ mert jobb esetben OutOfMemoryException ([PostgreSQL](../PostgreSQL.html) eseteben) rosszabb esetben kifogy a lockokbol az RDBMS ([Oracle](../Oracle.html) tipikusan).
*   A finally blockban mindenhol ellenorizgetni kell, kapkodni a hibakat, tovabbdobalni oket, logolni.
*   Az is fontos hogy hasznald a PreparedStatement-eket a parameterek meghatarozasara akkor is ha dinamikus SQL-t hasznalsz.

Hat par azokbol ami a legjobban fel szokott bosszantani. :)

# Mis-use

Egy erdekes JDBC kezeles egy ismert projectben: (csak a sema)
```
Statement s = null;
try{
s = con.createStatement();
...
ResultSet res = s.executeQuery();
...
s.close(); //a spec szerint ennek le kell zarnia a res-t is.
s=null;
} catch (Exception e){
logger.error("Anyam segits!", e);
}
if(s != null){
try{
s.close();
} catch (Exception e){
logger.warn("Sejehajj",e);
}
}
```
Szoval ez igen, vegulis felszabaditja az eroforrast akkor is ha valamilyen hiba keletkezik, csak aztan elhalgatja a hibat, azon kivul hogy logolt, a tranzakcio probal majd tovabbmenni. Jobb esetben nem sikerul, de en az ellenkezojetol jobban paraznek. Amugy kicsit [C](../C.html) sitlusra vall, mar nem az hogy elhalgatja, hanem az hogy Exception-t kap el. Bar mi is van [OOM](../OOM.html) eseten? Az nem [java.lang.Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html) leszamrmazott. Azert olyan van amikor kicsit nagy blobot szedunk lefele :)

Egy rovid levelvaltas a szerzovel, szerinte eleg jo es nem kell hogy jobb legyen, szerintem meg egyszer jol megszivja vele, de nekem ez nem faj.

# Mis-use 2

Nagyon sokat szivtam azzal hogy egy akkori kollegam [JDBC](../JDBC.html) trukkjeit (vagy [tak](../tak.html)jait) kijavitsam. A kovetkezokeppen mukodott.

1.   Az elozmeny: Termeszetesen irtak sajat connection-poolt. [Tomcat](../tomcat.html), [Oracle](../Oracle.html) db, egy nagyobb tablaval (nehany-tizezer sor).
1.   A Trukk: ket request jon a browserbol, az elsore nyit egy kapcsolatot es elinditja a query-t, a masodikra kipakolja. (ne kerdezd hogy ez miert jo)
1.   A gebasz: a query sokaig fut, meg a kliens kapcsolat is eleg lassu, nem biztos hogy a masodik lekerdezes is megjon. Sot valoszinuleg nem.
1.   A hibajelenseg: Valamiert meghal a [tomcat](../tomcat.html), neha az [oracle](../Oracle.html) is. Rovid nyomozas utan kiderul a fenti helyzet. (aztan fel ora orjonges)
1.   Az eslo megoldas: Atirom a connection pool-t hogy hasznalja a [JNDI](../JNDI.html)s [javax.sql.Datasource](http://docs.oracle.com/javase/7/docs/api/javax/sql/Datasource.html)-ot, aztan megprobalom valahogy atirni a mukodest. Perceken belul kiderul hogy joparszaz sort at kell irnom egyeb bugok miatt, vissza. Irtam egy kis wrappert a JDBC kore ami a lezarogatja a mar biztosan nem hasznalt eroforrasokat ([tak](../tak.html)).
1.   A vegso megoldas: eljottem, furodjenek a sajat sz@rukban :)
1.   Viszont akkor is van tanulsag: [php](../PHP.html) programmers, don't come to java town!

# Mis-use 3

Szerintem amit a [snipsnap](../SnipSnap.html) csinal a kapcsolatokkal, az is rossz, bar nagyon [windows](../Windows.html) juzer frendli, de monolitikus.

# Konkluzio

Ha nincs ra okod hogy [JDBC](../JDBC.html)t hasznalj, akkor [OR mapping](../OR%20Mapping.html), [hibernate](../Hibernate.html). Azt nem lehet igy elbaszni :)
Ha sebesseg kritikus alkalmazast irsz, (ilyen esetekben tenyleg nem annyira franko a [hibernate](../Hibernate.html) meg a hasonlok) de nem akarsz folosleges kodot irni, akkor is vannak hasznos eszkozok, peldaul a [spring](../spring.html) is ad egy hasznos frameworkot a [JDBC](../JDBC.html) kod ala.
