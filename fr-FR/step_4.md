## Contrôler le bateau

+ Tu vas contrôler le bateau avec ton souris. Ajoutez du code à ton bateau afin qu'il commence dans le coin inférieur gauche s'orientant vers le haut, et puis qu'il suive le pointeur de souris. **Teste ton code** pour verifier qu'il fat ce qu'il devrait faire.

\--- hints \--- \--- hint \--- Quand `le drapeau vert est cliqué`, tu dois envoyer ton bateau `à la position de départ` et `s'orienter vers le haut`. Ensuite, il faudra `s'orienter vers le pointeur de souris` et `avancer d'un pas`. Ceci doit être répété `indéfiniment`.

\--- /hint \--- \--- hint \--- Voici les blocs de code dont tu auras besoin: ![screenshot](images/boat-move-blocks.png) \--- /hint \--- \--- hint \--- Ton code devrait ressembler à ceci: ![screenshot](images/boat-move-code.png) \--- /hint \--- \--- /hints \---

+ Teste ton bateau en cliquant sur le drapeau et en déplaçant la souris. Est-ce que le bateau navigue vers la souris?
    
    ![screenshot](images/boat-mouse.png)
    
    ![screenshot](images/boat-pointer-test-anim.gif)

## \--- collapse \---

title: Si tu as des problèmes ...

## image: images/image.png

**Note:** There is currently a bug in Scratch which means your boat may not move towards the mouse pointer. If this happens, click the arrow on the `point towards` block and re-select `mouse-pointer`.

![screenshot](images/boat-bug.png) \--- /collapse \---

+ What happens if the boat reaches the mouse pointer? Try it.

+ To stop this from happening, you'll need to add an `if` block to your code, so that the boat only moves if it is more than 5 pixels away from the mouse.

\--- hints \--- \--- hint \--- The boat should only point towards the mouse pointer and move `if` the `distance to the mouse pointer` is `greater than 5 pixels`. \--- /hint \--- \--- hint \--- Here are the code blocks you'll need to add to the code for the boat: ![screenshot](images/boat-pointer-blocks.png) \--- /hint \--- \--- hint \--- This is what your code should look like: ![screenshot](images/boat-pointer-code.png) \--- /hint \--- \--- /hints \---

+ Test out your boat again to check whether the problem has been fixed.