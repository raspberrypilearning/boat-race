## Victoire!

--- task ---

Maintenant, ajoute une autre instruction `if`{:class="block3control"} au code de ton sprite de bateau afin que le joueur gagne lorsque le bateau arrive à l'île jaune.

Lorsque le bateau arrive sur l'île, le jeu doit dire "BRAVO !", Puis le jeu doit se terminer.

--- hints ---
--- hint --- 

Tu dois ajouter plus de blocs de code à l'intérieur de ta boucle `répéter indéfiniment`{:class="block3control"} pour que ton code continue de vérifier si le joueur a gagné :

`si`{:class="block3control"} le bateau `touche`{:class="block3sensing"} la couleur de l'île, tu dois `dire 'BRAVO !' pendant 2 secondes,`{:class="block3looks"}, puis `arrêtez tout`{:class="block3control"} pour terminer le jeu.

--- /hint ---

--- hint --- 

Voici les blocs de code dont tu auras besoin: ![sprite bateau](images/boat_resize.png)

```blocks3
say [BRAVO !] for (2) seconds

if <couleur touche [#FFFF99] ?> then
end

stop [tout v]

```
--- /hint --- 

--- hint ---

Voici à quoi devrait ressembler ton nouveau code: ![sprite bateau](images/boat_resize.png)

```blocks3
if <couleur touche [#FFFF99] ?> then
say [BRAVO !] for (2) seconds
stop [tout v]
end
```

N'oublie pas que ce nouveau code doit être dans la boucle `répéter indéfiniment`{:class="block3control"}.
--- /hint ---
--- /hints --- 
--- /task ---
