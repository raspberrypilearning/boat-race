## Unfall!

Dein Boot kann durch die braunen Holzbalken hindurch segeln! Das ändern wir jetzt.

## Arbeitsschritte { .check }

+ Du brauchst 2 Kostüme für dein Boot: Ein normales Kostüm, und eins für ein kaputtes Boot. Dupliziere das Boot Kostüm, und nenne sie 'Normal' und 'Kaputt'.

+ Klicke dein 'Kaputt' Kostüm und dann das 'Auswählen' Werkzeug an. Damit zerlegst du das Boot in Teile, bewegst und drehst sie. Lasse das Boot so aussehen als hätte es einen Unfall gebaut.

	![screenshot](images/boat-hit-costume.png)

+ Füge diesen Code zu deinem Boot hinzu, innerhalb der `wiederhole fortlaufend` {.blockcontrol} Schleife. Damit baut dein Boot jedes mal einen Unfall, wenn es einen der braunen Holzbalken berührt:

	```blocks
		falls <wird Farbe [#603C15] berührt?> dann
   			wechsle zu Kostüm [hit v]
   			sage [Oh nein!] für (1) Sek.
  			wechsle zu Kostüm [normal v]
  			setze Richtung auf (0 v)
   			gehe zu x:(-215) y:(-160)
		Ende
	```

	Dieser Code gehöhrt in die `wiederhole fortlaufend` {.blockcontrol} Schleife, sodass dein Code immer prüft, ob das Boot einen Unfall gebaut hat oder nicht.

+ Stelle sicher, dass dein Boot immer in dem 'Normal' Zustand startet.

+ Wenn du nun versuchst durch einen Holzbalken zu segeln, wirst du sehen, dass dein Boot kaputt geht und zum Start zurückkehrt.

	![screenshot](images/boat-crash.png)
