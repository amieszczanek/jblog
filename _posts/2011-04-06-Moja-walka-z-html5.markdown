---
layout: post
title: Moja-walka-z-html5
---
<aside id="img">
<img src="../../../../images/bhh5_xlargecover.jpg" alt="[Brian P.Hogan]" />
</aside>
<aside id="p">
&bdquo;In this book, you’re going to find out about all of the ways you can use 
HTML5 and CSS3 right now,even if your users don’t have browsers
that can support all of these features yet ...&rdquo;
</aside>

# {{ page.title }}  


## Html5

Moją walkę z Html5 zaczęłam od zmiany plików znajdujących sie w katalogu _layout w jBlogu.
Już na samym początku zaskoczyło mnie jak niewiele trzeba wiedzieć na temat html tworząc sam szablon.
W pierwszym etapie zamieniłam nagłówki w plikach.html. Bardzo przydatne są strony takie jak: [logooraphos](http://log.logographos.com/pl/design/html5/minikurs-htm5/new-tags-html/). Innym trafionym materiałem do nauki Html5 jest książka [Brian P.Hogan](http://pragprog.com/titles/bhh5/html5-and-css3)



## Etapy zmiany szablonu z Html4 na Html5
 
  * Zmiana nagłówka strony:  

Html4 było: 

************************************************************************
<"!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN">    
<"http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
************************************************************************ 

Html5 jest:  
 
****************************************************************************  
<"!DOCTYPE html">
**************************************************************************

  * Zmiana kodowania:    

Html4 było:  

*****************************************************************************  
<"html xmlns="http://www.w3.org/1999/xhtml">    
<"xml:lang="pl" lang="pl-pl"> 
<"meta http-equiv="content-type" content="text/html; charset="utf-8">  
*********************************************************************************  

Html5 jest:    

*******************************************************************************
<"html lang="pl">    
<"meta charset="utf-8">
**********************************************************************************

  * Na koniec dodałam elementy charakteryzujące używanie Html5 a mianowicie:  
    
***Navigacja*** może zawierać całe menu z linkami do głównych podstron, lub tylko np. linki wstecz/dalej.  
***Header*** służy przede wszystkim do określania nagłówka strony ale może określać nagłówek jakieś określonej sekcji. Wewnątrz tego znacznika znajdują się elementy, które standardowo tworzą nagłówek strony, a więc tytuł strony lub logo.  
***Section*** opisuje sekcję dokumentu, która może zawierać wszystkie możliwe inne znaczniki. Oczywiście, jedna sekcja może zawierać (nawet wielokrotnie) zagnieżdżone sekcje.  
***Article*** możemy używać tego tagu do określania komentarzy, postów itp. Jest on wielokrotnego użytku i nie jest zależny od strony.  
Tag ***Aside*** doskonale się nadaje jako element głównej treści, który ma być wyróżniony działa podobnie jak blocquote.  
***Footer*** oznacza stopkę, a więc znajdują się tam elementy które zazwyczaj umieszczamy na dole strony.

#Czy to nie jest piękne ;)#
