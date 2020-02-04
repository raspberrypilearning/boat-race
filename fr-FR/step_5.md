## Défi : Victoire!

\--- task \---

Now add another `if`{:class="block3control"} statement to your boat sprite's code so that the player wins when they make the boat arrive at the yellow island.

When the boat gets to the island, the game should say 'YEAH!', and then it should end.

\--- hints \--- \--- hint \---

Tu dois ajouter plus de blocs de code à l'intérieur de ta boucle `répéter indéfiniment`{:class="block3control"} pour que ton code continue de vérifier si le joueur a gagné :

`si`{:class="block3control"} le bateau `touche`{:class="block3sensing"} la couleur de l'île, tu dois `dire 'BRAVO !' pendant 2 secondes,`{:class="block3looks"}, puis `arrêtez tout`{:class="block3control"} pour terminer le jeu.

\--- /hint \--- \--- hint \---

Voici les blocs de code dont tu as besoin :

![bateau-sprite](images/boat_resize.png)

```blocks3
dire [BRAVO !] pendant (2) secondes

si <touching color [#FFFF99] ?> alors
fin

stopper [tout v]

```

\--- /hint \--- \--- hint \---

Voici à quoi devrait ressembler ton nouveau code :

![bateau-sprite](images/boat_resize.png)

```blocks3
si <touching color [#FFFF99] ?> alors
dire [BRAVO !] pendant (2) secondes
arrêter [tout v]
fin
```

N'oublie pas que ce nouveau code doit être dans la boucle `répéter indéfiniment`{:class="block3control"}.

\--- /hint \--- \--- /hints \--- \--- /task \---