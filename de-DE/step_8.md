## Hindernisse und Schübe

Dieses Spiel ist _viel_ zu leicht - Lass uns ein paar Dinge hinzufügen, um es spannender zu machen.

+ Als erstes füge ein paar 'Schübe' zu deinem Spiel, die das Boot beschleunigen. Ändere deinen Bühnen backdrop und füge ein paar weiße Schubpfeile hinzu.

	![screenshot](images/boat-boost.png)

+ Füge jetzt einen anderen Code zu deiner `wiederhole fortlaufend` {.blockcontrol} Schleife hinzu, sodass es 2 _extra_ Schritte macht, wenn es über einen Schubpfeil fährt.

	```blocks
		falls <wird Farbe [#FFFFFF] berührt?> dann
   			gehe (3) er-Schritt
		Ende
	```

+ Du kannst ein drehendes Tor erstellen, das dein Boot meiden soll. Füge ein neues Kostüm dazu und nenne es 'Tor'. So soll es aussehen:

	![screenshot](images/boat-gate.png)

	Die Farbe des Tors soll mit der Farbe der Holzbalken übereinstimmen.

+ Markiere den Drehpunkt des Kostüms.

	![screenshot](images/boat-center.png)

+ Füge den Code `wiederhole fortlaufend` {.blockcontrol} hinzu, damit sich das Tor sich langsam dreht.

+ Teste das Spiel. Jetzt sollst du ein drehendes Tor sehen, dass du lieber umschiffen sollst.

	![screenshot](images/boat-gate-test.png)
