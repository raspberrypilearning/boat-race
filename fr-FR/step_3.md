## Contrôler le bateau

\--- task \---

Add this code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![bateau-sprite](images/boat_resize.png)

```blocks3
lorsque le drapeau est cliqués
s'orienter en direction de (0)
aller à x: (-190) y: (-150)
répéter indéfiniment
s'orienter vers (pointeur de la souris v)
avancer de (1) pas
```

\--- /task \---

\--- task \---

**Teste ton code** en cliquant sur le drapeau vert et en déplaçant la souris. Le sprite du bateau se déplace-t-il vers le pointeur de la souris ?

![capture d'écran](images/boat-mouse.png)

\--- no-print \---

![capture d'écran](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![capture d'écran](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

Que se passe-t-il lorsque le bateau atteint le pointeur de la souris ? Essaie-le pour voir quel est le problème.

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

Teste à nouveau ton code pour vérifier si le problème est maintenant résolu.

\--- /task \---