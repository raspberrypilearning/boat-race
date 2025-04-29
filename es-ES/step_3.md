## Controlando el barco

\--- task \---

Add this code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![objeto barco](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
point towards (mouse-pointer v)
move (1) steps
```

\--- /task \---

\--- task \---

**Prueba tu código** haciendo clic en la bandera verde y moviendo el ratón. ¿El objeto barco se mueve hacia el puntero del ratón?

![captura de pantalla](images/boat-mouse.png)

\--- no-print \---

![captura de pantalla](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![captura de pantalla](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

¿Qué pasa cuando el barco llega al puntero del ratón? Pruébalo para ver cuál es el problema.

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

Prueba de nuevo tu código para comprobar si el problema se ha solucionado.

\--- /task \---