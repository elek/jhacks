---
creationDate        : 2005-04-05 20:57:47 +0200 
author              : admin 
title               : WTF/Date 
name                : WTF/Date 
layout              : wiki 
path                : WTF/Date 
date                : 2006-03-26 01:43:01 +0100 
version             : 1 
creator             : kocka 
---
Egy masik [java.util.Date](http://docs.oracle.com/javase/7/docs/api/java/util/Date.html) perverzio, amit [Zsoltk](../zsoltk.html) tett kozze regebben.
Magyon elnagyolva valahogy igy...

```

import java.sql.Connection;
// ... satobbi

public class DateUtil {
  public static Date getCurrentDate(Connection conn){
    Statement sta = conn.createStatement();
    ResultSet res = sta.executeQuery("select sysdate from dual");
    res.next();
    Date d = res.getDate(1);
    sta.close();
    return d;
  }
}
```

Kisse koltseges megoldas :), mire kiolvasod mar nem is annyi az ido. Kb mint atombombaval vadaszni verebre.
