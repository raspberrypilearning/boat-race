## Défi : Plus d'obstacles!
Pouvez-vous ajouter plus d'obstacles à votre jeu? Voici quelques idées :

+ Vous pourriez ajouter des marais verts à votre scène qui ralentiraient le joueur quand il les touche. Vous pouvez utiliser le bloc `attendre` {.blockcontrol} pour faire celà :

```blocks
	attendre (0.01) secondes
```

![screenshot](images/boat-algae.png)

+ Vous pourriez ajouter un objet qui se déplace, comme un tronc ou un requin!

![screenshot](images/boat-obstacles.png)

Ces blocs peuvent vous aider :

```blocks
	avancer de (1)
	rebondir si le bord est atteint
```

Si votre nouvel objet n'est pas brun, vous devrez ajouter à votre code de bateau :

```blocks
	si <<couleur [#603C15] touchée?> ou <[requin v] touché?>> alors
	fin
```
