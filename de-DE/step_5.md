## Gewonnen!

--- task --- Füge nun einen weiteren `wenn`{:class="block3control"} Anweisung zum Code deines Boot-Sprites hinzu, damit der Spieler gewinnt, wenn er das Boot auf der gelben Insel ankommt.

Wenn das Boot den Sandstrand erreicht, sollte das Spiel "JAAA!" sagen und enden.

--- hints ---
 --- hint --- Du musst deiner `wiederhole fortlaufend`{:class="block3control"} Schleife mehr Code hinzufügen, damit dein Code immer wieder prüft, ob das Spiel gewonnen worden ist:

`wenn`{:class="block3control"} das Boot `die gelbe Farbe der Insel <code>berührt`{:class="block3sensing"} lasse es `'JAAA!' sagen für 2 Sekunden`{:class="block3looks"} und anschließend `alles stoppen`{:class="block3control"}, um das Spiel zu beenden.
--- /hint ---
 --- hint --- Hier sind die Codeblöcke die du brauchen wirst: ![Boot-Figur](images/boat_resize.png)

```blocks3
sage [JAAA!] für (2) Sekunden

falls <wird Farbe [#FFFF99] berührt?> , dann
end

stoppe [alles v]
```

--- /hint --- --- hint --- So sollte dein neuer Programmiercode aussehen: ![Boot-Figur](images/boat_resize.png)

```blocks3
falls <wird Farbe [#FFFF99] berührt?> , dann 
sage [JAAA!] für (2) Sekunden
stoppe [alles v]
end
```

Vergiss nicht, dass dieser neue Code innerhalb deiner `wiederhole fortlaufend`{:class="block3control"} Schleife sein muss.
--- /hint ---
--- /hints --- --- /task ---