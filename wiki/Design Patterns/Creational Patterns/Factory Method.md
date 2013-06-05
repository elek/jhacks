---
creationDate: 1190898353142 
author: zmb 
contentAuthor: zmb 
title: Design Patterns/Creational Patterns/Factory Method 
contentUpdateDate: 1190902867037 
name: Design PatternsCreational PatternsFactory Method 
layout: wiki 
date: 1190902867037 
creator: karenin 
---
A lényeg az, hogy ne interface-re gondoljunk, hanem abstract osztályra.

Mondjuk van egy Jármű absztrakt osztályunk, aminek van createKerék() és cserélKerék() függvénye. Az előbbi absztrakt, hiszen a Szekérben más fajta kereket kreálunk, mint mondjuka Kocsi-ban. Viszont a cserélKerék egész konkrét, neki mindegy, hogy melyik kerék van, azt null-ra állítja, és aztán kicseréli azzal, hogy meghívja a createKerék() metódust, ami egy gyerek osztályban lesz implementálva. Tehát a factory method egy konkrét gyerek osztályban van implementálva, de már az absztrakt ős használja a gyümölcsét (nyilván itt is interface-en keresztül).

Na, ez nem biztos, hogy érthető lett, pedig valami ilyesmiről van szól.

Persze, ha már itt vagyunk, mondhatjuk azt is, hogy a Jármű nem is absztrakt, hanem ő is interface, de van valaki más, akin majd hivogatni akarja a jármű->createKerék()-et. Pl. az [Design Patterns/Creational Patterns/Abstract Factory](../../Design%20Patterns/Creational%20Patterns/Abstract%20Factory.html) egy szakajtó ilyen Factory Methodról szól.

Minimalista példa az érthetőség kedvéért.
{% highlight java %}
//a termek, amit a factory method eloallit
public interface Kerek \{
\}

//a termek ket megvalositasa
public class AutoKerek implements Kerek \{

	public String toString() \{
		return "autokerek";
	\}
\}

public class SzekerKerek implements Kerek \{

	public String toString() \{
		return "szekerkerek";
	\}
\}

//az os jarmu osztaly, ami hasznalja a factory methodot
abstract public class Jarmu \{
	protected Kerek kerek;
	
	public abstract Kerek createKerek();
	
	public void cserelKerek() \{
		kerek = createKerek();
	\}
	
\}

//ket konkret megvalositasa
public class Szeker extends Jarmu \{

	public Kerek createKerek() \{
		return new SzekerKerek();
	\}
	
	public String toString() \{
		return "Szeker, "+kerek;
	\}

\}

public class Auto extends Jarmu \{

	public Kerek createKerek() \{
		return new AutoKerek();
	\}

	public String toString() \{
		return "Auto, "+kerek;
	\}
\}

//vegul a tesztapp
public class Main \{
	
	public static void main(String[] args) \{
		Jarmu j1 = new Auto();
		Jarmu j2 = new Szeker();
		j1.cserelKerek();
		j2.cserelKerek();
		System.out.println(j1);
		System.out.println(j2);
	\}
\}

//es a kimenet
Auto, autokerek
Szeker, szekerkerek
{% endhighlight %}
