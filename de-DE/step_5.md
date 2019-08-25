## Einen Unfall bauen

\--- Aufgabe \--- Kannst du einen weiteren `falls`{:class="block3control"}-Block hinzufügen, so dass der Spieler gewinnt, wenn das Boot die Insel mit dem Sandstrand unten links erreicht?

Wenn das Boot den Sandstrand erreicht, sollte das Spiel "JAAA!" sagen und enden.

\--- hints \--- \--- hint \--- Du musst deiner `wiederhole fortlaufend`-Schleife mehr Code hinzufügen, damit dein Code immer wieder prüft, ob das Spiel gewonnen worden ist:

`Falls` das Boot die gelbe Farbe der Insel `berührt`, lasse es `'JAAA!' sagen für 2 Sekunden` und anschließend `alles stoppen`, um das Spiel zu beenden. \--- /hint \--- \--- hint \--- Hier sind die Codeblöcke die du brauchen wirst: ![Boot-Kostüm](images/boat_resize.png)

```blocks3
say [JAAA!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

\--- /hint \--- \--- hint \--- So sollte dein Programmiercode aussehen: ![Boot-Kostüm](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [JAAA!] for (2) seconds
stop [all v]
end
```

Vergiss nicht, dass dieser neue Code innerhalb deiner ` wiederhole fortlaufend ` {: class = "block3control"} Schleife sein muss. \--- / Hinweis \--- \--- / Hinweise \--- \--- / Aufgabe \---