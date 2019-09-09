## Obstacles et difficulté

Pour le moment, le jeu est **beaucoup** trop facile, tu vas donc ajouter quelques éléments pour le rendre plus intéressant.

Tout d'abord, tu vas ajouter des boosters pour accélérer le bateau.

\--- task \---

Modifie ton fond de scène en ajoutant des flèches de boosters blanches.

![capture d'écran](images/boat-boost.png)

\--- /task \---

\--- task \---

Ajoute maintenant plus de blocs de code à la boucle `répéter indéfiniment`{:class="block3control"} de ton bateau, de sorte que le sprite du bateau effectue trois pas supplémentaires lorsqu’il touche une flèche blanche. ![sprite bateau](images/boat_resize.png)

```blocks3
si <touching color [#FFFFFF] ?> alors
avancer de (3) pas
fin
```

\--- /task \---

\--- task \---

Teste ton jeu pour voir si tes nouvelles flèches de booster accélèrent le bateau.

\--- /task \---

Tu vas ensuite ajouter une porte en rotation que le bateau doit éviter.

\--- task \---

Ajoute un nouveau sprite qui ressemble à ceci et appelle-le 'porte':

![capture d'écran](images/boat-gate.png)

Assure-toi que la couleur du sprite de la porte est la même que celle des barrières en bois.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![porte](images/gate.png)

```blocks3
répéter indéfiniment
fin

tourner cw (1) degrés

quand le drapeau est cliqué
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

```blocks3
lorsque le drapeau est cliqué
répéter indéfiniment
tourner cw (1) degré
fin
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---