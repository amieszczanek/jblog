---
layout: post
title: Jak-powstaje-galeria-w-CSS
---

# {{ page.title }}

##Przykład Galerii, w której zdjęcie się powiększa, kiedy najedziemy na miniaturę


* Pierwszy etap

Sam początek wyświelenia galerii jest zupełnie prosty. Może nie wygląda to narazie zbyt pięknie ale efekt już jakiś widać. 
[Galeria1](http://sigma.inf.ug.edu.pl/~amieszczanek/blog/gallery/galeria1.html)
Jedyne co narazie zrobiłam to ustawiłam wysokość strony w której będa wyswietlane zdjęcia, jego wewnętrze marginesy oraz kolor tła do zdjęć.

* Drugi etap

Określiłam opływanie zdjęć do lewej (***float:left***), wysokość oraz szerokość zdjęć. Najważniejszym elementem jest dodanie 
***z-index***, które odpowiada za warstwowość linków. Z-index potrzebuje ustawienia *position*, przyjmuję ono wartość relative(pozwala na przesunięcie obrazka od np lewej i górnej krawędzi o wartość pixeli w stosunku do początkowej wartości pozycji) bądź absolute(pozwala przesunąć wybrany element w dowolną stronę względem wybranych brzegów strony).
W moim przykładzie zastosowałam ***position: relative***. Przykład: [Galeria2](http://sigma.inf.ug.edu.pl/~amieszczanek/blog/gallery/galeria2.html)

* Trzeci etap

Ta część jest dość prosta. Po prostu definiuje szerokość, wysokość, oraz inne stylizacje jaką chcemy dodać do tych miniatur. Wysokość i szerokość są konieczne. Reszta jest opcjonalna. Przykład: [Galeria3](http://sigma.inf.ug.edu.pl/~amieszczanek/blog/gallery/galeria3.html)

* Czwarty etap

Ostatni najwazniejszy etap, w którym nareszcie będzie coś widać. Przykład: [Galeria4](http://sigma.inf.ug.edu.pl/~amieszczanek/blog/gallery/galeria4.html). W tym etapie dodaję polecenie ***:hover***. Jest to pseudoklasa, która definiuje właściwości "najechanych" elementów, np. odnośników (linków). Dzięki temu po najechaniu na naszą miniaturę wyświetli się ona w innym położeniu.

Poniżej zamieszczam inny przykład galerii:

[Galeria Polaroid](http://sigma.inf.ug.edu.pl/~amieszczanek/blog/gallery/galeriaNowa2.html)



