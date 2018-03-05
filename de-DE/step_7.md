## Zeitfahren

Lass uns einen Timer zum Spiel hinzufügen. Damit soll der Spieler versuchen, so schnell wie möglich zur Wüsteninsel zu kommen.

+ Füge eine neue Variable  namens `Zeit` {.blockdata} zu deiner Bühne hinzu. Du kannst auch das Aussehen  der Variable ändern. Wenn du Hilfe brauchst schaue dir das 'Luftballons' Projekt an.

	![screenshot](images/boat-variable.png)

+ Füge diesen Code zu deiner __Bühne__ hinzu, sodass der Timer läuft bis das Boot an der Wüsteninsel ankommt:

	```blocks
		Wenn die grüne Flagge angeklickt
		setze [time v] auf [0]
		wiederhole fortlaufend
   			warte (0.1) Sek.
  			ändere [time v] um (0.1)
		Ende
	```

+ Das war's! Teste dein Spiel und versuch, so schnell wie möglich zur Wüsteninsel zu kommen.

	![screenshot](images/boat-variable-test.png)
