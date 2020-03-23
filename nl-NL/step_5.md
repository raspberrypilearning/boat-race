## Winnen!

--- task --- Voeg nu nog een `als`{:class="block3control"} blok toe aan de boot-sprite zodat de speler wint wanneer hij de boot op het gele eiland laten aankomen.

Wanneer de boot het eiland bereikt, moet het spel 'Ja!' zeggen en daarna zou het moeten stoppen.

--- hints ---
 --- hint --- Je moet een aantal code blokken toevoegen binnen de `herhaal`{:class="block3control"} lus zodat je code blijft controleren of de speler gewonnen heeft:

`als`{:class="block3control"} de boot `raakt`{:class="block3sensing"} de kleur van het eiland, dan moet de boot een `zeg 'Ja!' gedurende 2 seconden`{:class="block3looks"} uitvoeren en daarna een `stop alle`{:class="block3control"} om het spel te beëindigen.
--- /hint ---
 --- hint --- Dit zijn de codeblokken die je nodig hebt: ![boot-sprite](images/boat_resize.png)

```blocks3
say [Ja!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]
```

--- /hint --- --- hint --- Zo zou je code er uit moeten zien: ![boot-sprite](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [Ja!] for (2) seconds
stop [all v]
end
```

Vergeet niet dat deze nieuwe code in de `herhaal`{:class="block3control"} lus moet staan.
--- /hint ---
--- /hints --- --- /task ---