## Einen Unfall bauen

\--- Aufgabe \--- Füge nun einen weiteren `wenn`{:class="block3control"} Anweisung zum Code deines Boot-Sprites hinzu, damit der Spieler gewinnt, wenn er das Boot auf der gelben Insel ankommt.

Wenn das Boot den Sandstrand erreicht, sollte das Spiel "JAAA!" sagen und enden.

\--- hints \--- \--- hint \--- Du musst deiner `wiederhole fortlaufend`-Schleife mehr Code hinzufügen, damit dein Code immer wieder prüft, ob das Spiel gewonnen worden ist:

`Falls` das Boot die gelbe Farbe der Insel `berührt`, lasse es `'JAAA!' sagen für 2 Sekunden` und anschließend `alles stoppen`, um das Spiel zu beenden. \--- /hint \--- \--- hint \--- Hier sind die Codeblöcke die du brauchen wirst: ![Boot-Kostüm](images/boat_resize.png)

```blocks3
sag [JAAA!] für (2) Sekunden
wenn <touching color [#FFFF99] ?> dann
ende
stoppe [alles v]

```

\--- /hint \--- \--- hint \--- So sollte dein Programmiercode aussehen: ![Boot-Kostüm](images/boat_resize.png)

```blocks3
wenn <touching color [#FFFF99] ?> dann
sage [JAAA!] für (2) Sekunden
stoppe [alles v]
ende
```

Vergiss nicht, dass dieser neue Code innerhalb deiner ` wiederhole fortlaufend ` {: class = "block3control"} Schleife sein muss. \--- / Hinweis \--- \--- / Hinweise \--- \--- / Aufgabe \---