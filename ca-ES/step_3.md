## Control del vaixell

\--- task \---

Add this code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![icona-vaixell](images/boat_resize.png)

```blocks3
quan es fa clic a la bandera
apunta en la direcció (0)
ves a x: (-190) y: (-150)
per sempre
apunta cap a (punter del ratolí v)
mou (1) passa
```

\--- /task \---

\--- task \---

** Prova el teu codi ** fent clic a la bandera verda i movent el ratolí. El dibuix del vaixell es mou cap al punter del ratolí?

![captura de pantalla](images/boat-mouse.png)

\--- no-print \---

![captura de pantalla](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![captura de pantalla](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

Què passa quan el vaixell arriba al punter del ratolí? Prova-ho per veure quin és el problema.

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

Prova el teu codi de nou per comprovar si el problema està arreglat.

\--- /task \---