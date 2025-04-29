## Controllare la barca

\--- task \---

Add this code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![sprite barca](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
point towards (puntatore del mouse v)
move (1) steps
```

\--- /task \---

\--- task \---

**Prova il tuo codice** cliccando sulla bandiera verde e spostando il mouse. La barca si muove verso il puntatore del mouse?

![schermata](images/boat-mouse.png)

\--- no-print \---

![schermata](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![schermata](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

Cosa succede quando la barca raggiunge il puntatore del mouse? Prova per vedere qual è il problema.

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

Fai un'altra prova per vedere se il problema è stato risolto.

\--- /task \---