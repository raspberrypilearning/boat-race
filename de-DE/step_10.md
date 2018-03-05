--- challenge ---

## Herausforderung: Mehr Boote!
Kannst du das Spiel so ausbauen, dass zwei Spieler das gleichzeitig spielen können.

+ Dupliziere das Boot, nenne es 'Spieler 2' und ändere seine Farbe.

![screenshot](images/boat-p2.png)

+ Ändere die Startposition des Spieler 2, indem du diesen Code änderst:

```blocks
	gehe zu x:(-190) y:(-150)
```

+ Lösche den Code für die Maussteuerung:

```blocks
	falls <(Entfernung von [Mauszeiger v]) > [5]> dann
   		drehe dich zu [Mauszeiger v]
   		gehe (1) er-Schritt
	Ende
```

...und ersetze ihn mit dem Code für die Tastatursteuerung mit den Pfeiltasten.

Mit diesem Code wird das Boot vorwärts bewegt:

```blocks
	falls <Taste [Pfeil nach oben v] gedrückt?> dann
   		gehe (1) er-Schritt
	Ende
```

Du brauchst auch den Code zum `drehen`{:class="blockmotion"} des Boots, wenn der Spieler auf die Pfeiltasten 'Links' oder 'Rechts' drückt.
