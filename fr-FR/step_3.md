## Contrôler le bateau

Le joueur contrôlera le sprite du bateau avec la souris.

\--- task \---

Ajoute du code à ton bateau afin qu'il commence dans le coin inférieur gauche, orienté vers le haut, et puis qu'il suive le pointeur de souris.

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

What happens when the boat reaches the mouse pointer? Try it out to see what the problem is.

\--- /task \---

\--- task \---

Pour que cela ne se produise pas, tu dois ajouter un bloc `si`{:class="block3control"} à ton code, de sorte que ton sprite ne se déplace que si il est à plus de 5 pixels du pointeur de la souris.

\--- hints \--- \--- hint \---

Le bateau ne doit pointer que vers le pointeur de la souris et se déplacer `si`{:class="block3control"} la `distance au pointeur de la souris`{:class="block3sensing"} est `supérieure à 5 pixels`{:class="block3operators"}.

\--- /hint \--- \--- hint \---

Voici les blocs de code que tu dois ajouter au code pour le sprite bateau :

![bateau-sprite](images/boat_resize.png)

```blocks3
si < [ ] > [ ] > alors

(distance de (pointeur de souris v))
```

\--- /hint \--- \--- hint \---

Voici à quoi ton code devrait ressembler :

![bateau-sprite](images/boat_resize.png)

```blocks3
lorsque le drapeau est cliqué
s'orienter en direction de (0)
aller à x: (-190) y: (-150)
répéter indéfiniment
si <(distance de (pointeur de souris v)) > [5]> alors
s'orienter vers (pointeur de souris v)
avancer de (1) pas
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Teste à nouveau ton code pour vérifier si le problème est maintenant résolu.

\--- /task \---