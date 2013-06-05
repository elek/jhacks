---
creationDate: 1112727467778 
author: kocka 
contentAuthor: kocka 
title: WTF/Date 
contentUpdateDate: 1112727525399 
name: WTFDate 
layout: wiki 
date: 1112727525399 
creator: kocka 
---
Egy masik  perverzio, amit [Zsoltk](../zsoltk.html) tett kozze regebben.
Magyon elnagyolva valahogy igy...

{% highlight java %}

import java.sql.Connection;
// ... satobbi

public class DateUtil \{
  public static Date getCurrentDate(Connection conn)\{
    Statement sta = conn.createStatement();
    ResultSet res = sta.executeQuery("select sysdate from dual");
    res.next();
    Date d = res.getDate(1);
    sta.close();
    return d;
  \}
\}
{% endhighlight %}

Kisse koltseges megoldas :), mire kiolvasod mar nem is annyi az ido. Kb mint atombombaval vadaszni verebre.
