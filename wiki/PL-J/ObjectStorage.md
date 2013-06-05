---
creationDate: 1103712506784 
author: kocka 
contentAuthor: kocka 
title: PL-J/ObjectStorage 
contentUpdateDate: 1114033564645 
name: PL-JObjectStorage 
layout: wiki 
date: 1114033564645 
creator: kocka 
---
A [PL-J/Devtools](../PL-J/DevTools.html) for utan az ObjectStorage otlet is kicsit kanyarodik. Egy kis kiegeszites lenne a forkolt projecten.

{% highlight java %}

import java.util.Date;

/**
 * @plj.rdbmstype name="jPerson"
 */
public class Person \{
 Date birthDate;
 String name;
 public Date getBirthDate() \{ return birhthDate; \}
 public void setBirthDate(Date newBirthDate) \{ birthDate = newBirthDate; \}
 public String getName() \{ return name; \}
 public void setName(String newName) \{ name = newName; \}
\}

{% endhighlight %}

Generalt kodok:
{% highlight java %}
create type jPerson

create function jPerson_getName(jPerson) returns varchar as 
'
class=PersonHelper
method=jPerson_getName
' language 'PL-J' immutable

-- satobbi
{% endhighlight %}

remelem az otletet ertitek.
Na most mivel a funkciok _immutable_k ezert konnyen keszithetunk rajuk indexet, azaz a sebessegbol valoszinuleg nem veszitunk valami sokat, cserebe kapunk egy erdeks cuccot.

Konkretan a pelda medint kicsit butus, de legalab ecceru.

Lasd meg: [PL-J/DevTools](../PL-J/DevTools.html)
