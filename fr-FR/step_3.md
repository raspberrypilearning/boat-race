## Contrôler le bateau

Le joueur contrôlera le sprite du bateau avec la souris.

--- task --- Ajoute du code au sprite du bateau pour qu'il commence dans le coin inférieur gauche pointant vers le haut et suit le pointeur de la souris.

![bateau-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
point towards (pointeur de la souris v)
move (1) steps
```

--- /task ---

--- task ---

**Teste ton code** en cliquant sur le drapeau vert et en déplaçant la souris. Le sprite du bateau se déplace-t-il vers le pointeur de la souris?

![capture d'écran](images/boat-mouse.png)

--- no-print --- ![screenshot](images/boat-pointer-test-anim.gif) --- /no-print ---

--- print-only --- ![screenshot](images/boat-pointer-test-anim.png) --- /print-only ---

--- /task ---

--- task ---

Que se passe-t-il lorsque le bateau atteint le pointeur de la souris? Essaie-le pour voir quel est le problème.

--- /task ---

--- task ---

Pour que cela ne se produise pas, tu dois ajouter un bloc `si`{: class = "block3control"} à ton code, de sorte que ton sprite ne se déplace que si il est à plus de 5 pixels du pointeur de la souris.

--- hints ---
 --- hint --- Le bateau ne devrait pointer que vers le pointeur de la souris et déplacer `si`{:class="block3control"} la `distance vers le pointeur de la souris`{:class="block3sensing"} est `supérieur à 5 pixels`{:class="block3operators"}. --- /hint --- --- hint --- Voici les blocs de code que tu dois ajouter au code du sprite du bateau: ![bateau-sprite](images/boat_resize.png)

```blocks3
si < [ ] > [ ] > alors

(distance de (pointeur de souris v))
```

---/hint--- ---hint--- Voici a quoi devrait ressembler ton code: ![sprite bateau](images/boat_resize.png)

```blocks3
lorsque le drapeau est cliqué
s'orienter en direction de (0)
aller à x: (-190) y: (-150)
répéter indéfiniment
si <(distance de (pointeur de souris v)) > [5]> alors
s'orienter vers (pointeur de souris v)
avancer de (1) pas
```

--- /hint ---
--- /hints ---

--- /task ---

--- task ---

Teste à nouveau ton code pour vérifier si le problème est maintenant résolu.

--- /task ---