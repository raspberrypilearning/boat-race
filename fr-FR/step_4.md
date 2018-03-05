## Collision!

Votre bateau peut naviguer à travers les barrières en bois! Arrangeons cela.

+ Vous aurez besoin de 2 costumes pour votre bateau, un costume normal et un pour quand le bateau est détruit. Dupliquez votre costume de bateau et nommez-les 'bateau' et 'bateau détruit'.

+ Cliquez sur le costume 'bateau détruit' et choisissez l'outil 'Sélectionner' pour saisir et déplacer les morceaux du bateau et les faire tourner autour. Faites semblant que votre bateau est détruit.

	![screenshot](images/boat-hit-costume.png)

+ Ajoutez ce code à votre bateau, à l'intérieur de la boucle 'répéter indéfiniment' {.blockcontrol}, pour qu'il se détruise lorsqu'il touche des morceaux en bois :

	```blocks
		si <couleur [#603C15] touchée?> alors
		   basculer sur costume [bateau détruit v]
		   dire [Noooooon!] pendant (1) secondes
		   basculer sur costume [bateau v]
		   s'orienter à (0 v)
		   aller à x:(-215) y:(-160)
		fin
	```

	Ce code est à l'intérieur de la boucle 'répéter indéfiniment' {.blockcontrol} pour que votre code vérifie continuellement si le bateau entre en collision.

+ Vous devriez aussi vous assurer que votre bateau commence toujours sur le costume 'bateau'.

+ Maintenant si vous essayez d'entrer en collision avec une barrière en bois, vous devriez voir que votre bateau se détruit puis revient au début.

	![screenshot](images/boat-crash.png)
