---
layout: post
title: Jak-powstaje-galeria-w-CSS
---

# {{ page.title }}

##Przykład Galerii, w której zdjęcie się powiększa, kiedy najedziemy na miniaturę


* Pierwszy etap

Sam początek wyświelenia galerii jest zupełnie prosty. Może nie wygląda to narazie zbyt pięknie ale efekt już jakiś widać. 
[Galeria1](http://sigma.inf.ug.edu.pl/~amieszczanek/blog/gallery/galeria1.html)
Jedyne co narazie zrobiłam to ustawiłam wielkość zdjęcia miniaturka oraz wielkość zdjęcia wyświetlanego.
<pre>
{% highlight ruby %}
.Galeria{
	width: 60%;
}
.zdjecie img{
	width: 150px;
	height: 120px;
}
.zdjecie span img{ 
	width: 300px;
	height: 340px;
}
{% endhighlight %}
</pre>

* Drugi etap

W tym etapie dodałam *position* dla całej galerii oraz dla zdjęć zmieniających pozycję. Dodatkowo ustawiłam marginesy zewnętrzne
jak i wewnętrzne oraz czcionkę z informacją o zdjęciu.
<pre>
{% highlight ruby %}
.Galeria{
	position: relative;
	}
.zdjecie img{
	padding-top: 2px;
	margin: 0 5px 5px 0;
}
.zdjecie span{
	position: absolute;
	background-color: #FFCC99;
	padding: 5px;
	left: -1000px;
	border: 1px ridge #804000;
	visibility: hidden;
	color: black;
	text-decoration: none;
	font-family: "Monotype Corsiva";
	font-size: 15px;
}
.zdjecie span img{ 
	border-width: 0;
	padding: 2px;
}
{% endhighlight %}
</pre>

Przykład: [Galeria2](http://sigma.inf.ug.edu.pl/~amieszczanek/blog/gallery/galeria2.html)

* Trzeci etap

Na tym etapie zajełam się akcją tzn dodałam tag *hover*(pseudoklasa, która definiuje właściwości "najechanych" elementów, np. odnośników (linków))
oraz *z-index*, które odpowiada za warstwowość zdjęć. 
<pre>
{% highlight ruby %}
.zdjecie:hover img{
	
	border-width: 2px;
	border-color: #804000 #804000 #804000 #9D4F4F;
}
.zdjecie:hover span{ 
	visibility: visible;
	top: 0;
	left: 390px;
	z-index: 50;
}
{% endhighlight %}
</pre>

Przykład: [Galeria3](http://sigma.inf.ug.edu.pl/~amieszczanek/blog/gallery/galeria3.html)

* Czwarty etap

W tym etapie znajduję się tylko kosmetyka. Dodałam jedynie tła dla galerii oraz strony, aby było ładniejsze.
Przykład: [Galeria4](http://sigma.inf.ug.edu.pl/~amieszczanek/blog/gallery/galeria4.html).
Poniżej zamieszczam inny przykład galerii:

[Galeria Polaroid](http://sigma.inf.ug.edu.pl/~amieszczanek/blog/gallery/galeriaNowa2.html)



