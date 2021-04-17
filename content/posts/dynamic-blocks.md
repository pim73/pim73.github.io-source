---
title: "Dynamic Blocks"
date: 2021-04-16T07:40:06+02:00
categories: ["Kodowanie"]
tags: ["emacs","orgmode","lifehacks"]
---
### Problem
 
 Zamierzam stworzony w orgmode outline przekrztałcić w tabelę. Dotychczas bez problemu korzystałem z `column view`. Taka funkcja   okazywała się przydatna, gdyż w przejrzysty sposób prezentuje te dane, które chcę wyeksponować. Niestety nie ma możliwości        wyeksportowania takiego widoku. 
 
 ### Rozwiązanie problemu
 Rozwiązaniem okazuje się istniejąca funkcja `Dynamic Blocks`.
 
 Wcześniej zdefiniować `Dynamic Blocks` w pliku `.emacs`
 
 ```lisp
 (org-dynamic-block-define "columnview" 'org-insert-columns-dblock)
 (org-dynamic-block-define "aggregate" 'org-insert-dblock:aggregate)
 ```
 Teraz wystarczy umieścić kursor na nagłówku, z którego punktów chcemy utworzyć tabelę i wywołać funkcję za pomocą skrótu:
 
 `C-c C-x x columnview`
 
 Pod nagłówkiem utworzona jest tablica, z którą można zrobić wszystko, co się chce. Co ważne, nie przekształca to w żaden sposób   podpunktów samego nagłówka.
