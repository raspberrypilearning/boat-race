## Botsen!

Op dit moment kan de boot-sprite gewoon door de houten barrières varen! Je gaat dat nu repareren.

--- task ---

Je hebt twee uiterlijken voor je boot nodig, een normaal uiterlijk en een voor wanneer de boot crasht. Maak een kopie van het huidige uiterlijk en noem één uiterlijk 'normaal' en de andere 'raak'.

--- /task ---

--- task ---

Klik op je 'raak'-uiterlijk en gebruik het **Selectie** hulpmiddel om stukjes van de boot te pakken en deze vervolgens te verplaatsen en te draaien zodat het lijkt dat de boot in stukken is gevallen.

![screenshot](images/boat-hit-costume-annotated.png)

--- /task ---

--- task ---

Voeg nu code aan je boot toe zodat deze crasht en uit elkaar valt wanneer deze de bruine houten hindernis raakt.

--- hints ---
--- hint --- Je moet code-blokken toevoegen in je `herhaal`{:class="block3control"} lus zodat de code blijft controleren of de boot-sprite is gecrasht en als deze is gecrasht, moet de code de positie van de boot-sprite opnieuw instellen.

`als`{:class="block3control"} de boot de bruine kleur van het hout `raakt`{:class="block3sensing"}, moet je `veranderen naar het raak uiterlijk`{:class="block3looks"} en `zeg Neeeeeee! gedurende 2 seconden`{:class="block3looks"}, en dan `verander terug naar het normale uiterlijk`{:class="block3looks"}. Ten slotte moet je `richt naar boven`{:class="block3motion"} en `ga naar de startpositie`{:class="block3motion"}.

--- /hint --- 
--- hint --- 

Dit zijn de codeblokken die je nodig hebt: 

![boot-sprite](images/boat_resize.png)

```blocks3
als <touching color [ ] ?> dan
einde

ga naar x: (-190) y: (-150)

verander uiterlijk naar (raak v)

richt naar (0) graden

verander uiterlijk naar (normaal v)

zeg [Neeeeeee! ] (2) sec.
```

--- /hint --- 
--- hint --- 

Zo zou je code er uit moeten zien: 

![boot-sprite](images/boat_resize.png)

```blocks3
wanneer op groene vlag wordt geklikt
richt naar (0) grden
ga naar x: (-190) y: (-150)
herhaal
als <(afstand tot (muisaanwijzer v)) > [5]> dan
richt naar (muisaanwijzer v)
neem (1) stappen
end
als <touching color [#663b00] ?> dan
verander uiterlijk naar (raak v)
zeg [Neeeeee!] (2) sec.
verander uiterlijk naar (normaal v)
richt naar (0) graden
ga naar x: (-190) y: (-150)
end
```

--- /hint --- 
--- /hints ---

--- /task ---

--- task ---

Je moet ook code toevoegen die ervoor te zorgt dat je boot-sprite altijd begint met een 'normaal' uiterlijk.

Test je code opnieuw. Als je nu probeert om de boot door een houten barrière te varen moet de boot crashen en weer naar de startpositie terugkeren.

![screenshot](images/boat-crash.png)

--- /task ---