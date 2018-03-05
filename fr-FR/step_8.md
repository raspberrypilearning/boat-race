## Obstacles et difficulté

Ce jeu est trop facile, ajoutons des choses pour le rendre plus intéressant.

+ D'abord, ajoutons quelques zones d'accélération à votre jeu qui accéléreront le bateau lorsqu'il les traversera. Modifiez votre scène et ajoutez quelques flèches blanches.

	![screenshot](images/boat-boost.png)

+ Vous pouvez maintenant ajouter du code à la boucle `répéter indéfiniement` {.blockcontrol} de votre bateau pour qu'il se déplace de trois pixels supplémentaires en touchant une flèche blanche.

	```blocks
		si <couleur [#FFFFFF] touchée?> alors
		   avancer de (3)
		fin
	```

+ Vous pouvez aussi ajouter une porte tournante que votre bateau doit éviter. Ajoutez un nouveau lutin appelé 'porte' qui ressemble à ceci :

	![screenshot](images/boat-gate.png)

	Assurez-vous que la porte est de la même couleur que les autres barrières en bois.

+ Définissez le centre du lutin 'porte'.

	![screenshot](images/boat-center.png)

+ Ajoutez le code à votre porte pour la faire tourner lentement dans le bloc 'répéter indéfiniment' {.blockcontrol}.

+ Testez votre jeu. Vous devriez maintenant avoir une porte tournante que vous devez éviter.

	![screenshot](images/boat-gate-test.png)
