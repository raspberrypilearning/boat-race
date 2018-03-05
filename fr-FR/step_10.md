## Défi : Plus de bateaux!
Pouvez-vous transformer votre jeu en course entre 2 joueurs?

+ Dupliquez le bateau, renommez le 'Joueur 2' et changez sa couleur.

![screenshot](images/boat-p2.png)

+ Changez la position de départ du Joueur 2, en changeant ce code:

```blocks
	aller à x:(-190) y:(-150)
```

+ Supprimez le code qui utilise la souris pour contrôler le bateau :

```blocks
		si <(distance de [pointeur de souris v]) > [5]> alors
		   s'orienter vers [pointeur de souris v]
		   avancer de (1)
		fin
```

...Et remplacez le code pour contrôler le bateau en utilisant les touches de direction.

Ceci est le code pour faire avancer le bateau avec les flèches :

```blocks
	si <touche [flèche haut v] pressée?> alors
   	avancer de (1)
	fin
```

Vous aurez aussi besoin du bloc `tourner` {.blockmotion} pour que le bateau tourne quand les touches de direction gauches et droites sont appuyées.
