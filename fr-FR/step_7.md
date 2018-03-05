## Course contre la montre

Ajoutons un minuteur à votre jeu, pour que le joueur arrive à l'île déserte le plus rapidement possible.

+ Ajoutez une nouvelle variable appelée `temps`{:class="blockdata"} à votre scène. Vous pouvez aussi changer la présentation de votre nouvelle variable. Si vous avez besoin d'aide, regardez le projet 'SOS Fantômes'.

	![screenshot](images/boat-variable.png)

+ Ajoutez ce code à votre scène pour que le minuteur compte jusqu'à-ce que le bateau atteigne l'île déserte :

	```blocks
		quand le drapeau vert pressé
		[temps v] prend la valeur [0]
		répéter indéfiniment
		   attendre (0.1) secondes
		   [temps v] prend la valeur (0.1)
		fin
	```

+ C'est ça! Testez votre jeu et essayez d'aller le plus rapidement possible à l'île déserte!

	![screenshot](images/boat-variable-test.png)
