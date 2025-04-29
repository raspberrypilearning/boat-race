## Controlar o barco

\--- task \---

Add this code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![ator barco](images/boat_resize.png)

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

** Testa o teu código ** clicando na bandeira verde e movendo o rato. O actor barco move-se em direção ao ponteiro?

![captura de ecrã](images/boat-mouse.png)

\--- no-print \---

![captura de ecrã](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![captura de ecrã](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

O que é que acontece quando o barco atinge o ponteiro do rato? Experimenta para ver qual é o problema.

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

Testa o teu código novamente para verificar se o problema está resolvido.

\--- /task \---