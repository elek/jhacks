---
creationDate: 1104483045681 
author: karenin 
contentAuthor: karenin 
title: junit 
contentUpdateDate: 1196678176504 
name: junit 
layout: wiki 
date: 1196678176504 
creator: kocka 
---
![image](http://www.junit.org/images/junitlogo.gif)(http://junit.org/)

Szoval a junit alapveto eszkoz egy onmagara valamit is ado programozo kezeben. Bar eleg egyszerucske. A junit teszteket hajt vegre. Valahogy igy:

{% highlight java %}

class TestWhatever extends TestCase \{
    //Ez hivodik meg a tesztek elott
    public void setUp() \{\}
    //Es a tesztek utan
    public void tearDown() \{\}
    //Es a tesztjeid csupa public es test-tel kezdodo metodusok, pl
    publi void testAkarmi() \{
        ...
    \}
\}

{% endhighlight %}

A kicsit ujabb es modernebb __junit 4__ a [java 1.5](java%201.5.html) [annotations](annotations.html) feature-re epit, ezzel kb igy nez ki egy teszt:

{% highlight java %}
class TestWhatever \{ //nem am extends, pojo baszkikaim!!!
    @Test // ez a teszt maga
    public void something() \{
    ...
    \}
    @Before
    public void elottehivdMarMegLecci() \{
    \}
\}
{% endhighlight %}

Szoval a jo oreg junit utannaeredt a fiatal tronfosztoknak mint a [testng](testng.html). Ha lassan is. A teljesen uj [pojo](pojo.html) teszteknek szerintem az lesz a vege hogy paran beleirjak a teszteket az objektumokba magaba, tovabblepve pedig majd az eles metodusok teszt metodusokat is fognak hivni. En barmilyen allatsagot el tudok kepzelni :)

Az [IDE](IDE.html)-k altalaban tartalmaznak valamilyen supportot a junit futtatashoz, az [eclipse](Eclipse.html)-ben ez nagyon rulla, a tobbit nem tudom, de itt egy link hozza: http://www.junit.org/news/ide/index.htm (NetBeans pl. már simán kezeli)

A junit mindenféle portjai:

*   [dbunit](dbunit.html)
*   [httpunit](httpunit.html)
*   satobbiunit



Nekem a kedvencem az amikor egyszerűen csinálsz egy spring context-et és abból szedsz ki bean-eket amiken meghívhatsz a tesztekben metódusokat. Nagyon könnyen ujrafelhasználhatóvá teszi a teszteket.



A 4.1-es verzio ujitasa kozott a leglenyegesebb talan a [Test/Categorization](Test/Categorization.html), szinten [java](java.html) [annotations](annotations.html) segitsegevel. Sok uj es modern dolog van a [4.1](Missing.html)ben csak sajnos semmi sem tamogatja per pillanat. Se [eclipse](Eclipse.html), se [maven](maven.html). Tul nagy szakitas volt a regi apival talan, de remelem ez lassan tovabb fejlodik.



Cikkek:
*   [Testing Java in an Object-Oriented Way](http://today.java.net/pub/a/today/2006/03/28/testing-java-object-oriented.html) (advanced)
*   [JUnit Reloaded](http://today.java.net/lpt/a/341)
*   [Twik összefolgalója a 3->4-ról.](http://pcjuzer.blogspot.com/2007/12/junit-4.html)

Lasd meg: [XP](XP.html) [test](test.html)




