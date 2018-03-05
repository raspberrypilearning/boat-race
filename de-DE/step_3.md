## Boot steuern

+ Wenn du vom Lehrer den Zugang zum 'Resources' Verzeichnis bekommen hast, klicke auf "Figur aus einer Datei laden" und füge die Bilddatei 'boat.png' hinzu. Verkleinere die Figur und stelle sie auf die Startposition.

	![screenshot](images/boat-boat.png)

	Wenn du das boat.png image nicht hast, mal dein eigenes Boot!

+ Du wirst das Boot mit deiner Maus Steuern. Füge diesen code zu deinem boot hinzu:

	```blocks
		Wenn die grüne Flagge angeklickt
		setze Richtung auf (0 v)
		gehe zu x:(-190) y:(-150)
		wiederhole fortlaufend
			drehe dich zu [Mauszeiger v]
   			gehe (1) er-Schritt
   		Ende
	```

+ Teste dein Boot, indem du die Flagge anklickst und die Maus bewegst. Segelt das Boot in Richtung der Maus?

	![screenshot](images/boat-mouse.png)

+ Was passiert wenn das Boot den Mauszeiger berührt?

	Um es zu verhindern, füge ein `falls`{:class="blockcontrol"} Skript zu deinem Code hinzu, sodass sich das Boot nur bewegt, wenn es mehr als 5 Pixel von der Maus entfernt ist.

	![screenshot](images/boat-pointer.png)	

+ Teste dein Boot wieder und überprüfe, ob das Problem gelöst ist.
