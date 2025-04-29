## Tekneyi kontrol etme

\--- task \---

Add this code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![tekne-görüntüsü](images/boat_resize.png)

```blocks3
bayrak (0)
yönünde
noktaya tıkladığında x: (-190) y: (-150)
sonsuza kadar
noktaya (fare imleci v)
hareket ettirin (1)
```

\--- /task \---

\--- task \---

Yeşil bayrağa tıklayın ve fareyi hareket ettirerek **kodunuzu test edin**. Tekne sprite'ı fare imlecine doğru hareket ediyor mu?

![ekran görüntüsü](images/boat-mouse.png)

\--- no-print \---

![ekran görüntüsü](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![ekran görüntüsü](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

Tekne fare imlecine ulaşırsa ne olur? Dene ve sorunun ne olduğunu gör.

\--- /task \---

\--- task \---

Add code to the boat sprite so it only point towards the mouse pointer and moves `if`{:class="block3control"} the `distance to the mouse pointer`{:class="block3sensing"} is `greater than 5 pixels`{:class="block3operators"}.

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
+if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

\--- /task \---

\--- task \---

Sorunun çözülüp çözülmediğini kontrol etmek için kodunuzu tekrar test edin.

\--- /task \---