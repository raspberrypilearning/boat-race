## Direction du bateau

+ Si votre leader de club vous a donné un dossier 'Ressources', cliquez 'importer un lutin depuis un fichier' et ajouter l'image 'boat.png'. Vous devriez faire rétrécir le lutin et y définir la position de départ.

	![screenshot](images/boat-boat.png)

	Si vous n'avez pas l'image de 'boat.png', vous pouvez dessiner votre propre bateau!

+ Vous allez contrôler le bateau avec votre souris. Ajoutez ce code à votre bateau:

	```blocks
		quand le drapeau vert pressé
		s'orienter à (0 v)
		aller à x:(-190) y:(-150)
		répéter indéfiniment
		   s'orienter vers [pointeur de souris v]
		   avancer de (1)
		fin
	```

+ Testez votre jeu en cliquant sur le drapeau et en déplaçant la souris. Le bateau navigue-t-il vers la souris?

	![screenshot](images/boat-mouse.png)

+ Qu'est-ce qui arrive si le bateau atteint le curseur de souris?

	Pour arrêter ce comportement, vous devrez ajouter le bloc `si`{:class="blockcontrol"} à votre code pour que le bateau se déplace seulement si votre souris est à plus de 5 pixels.

	![screenshot](images/boat-pointer.png)

+ Testez votre bateau de nouveau, vérifiez si le problème a été résolu.
