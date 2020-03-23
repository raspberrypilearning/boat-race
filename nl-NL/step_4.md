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

`als`{:class="block3control"} de boot de bruine kleur van het hout `raakt`{:class="block3sensing"}, moet je `veranderen naar het raak uiterlijk`{:class="block3looks"} en `zeg Neeeeeee! gedurende 2 seconden`{:class="block3looks"}, en dan `verander terug naar het normale uiterlijk`{:class="block3looks"}. Ten slotte moet je `richt naar boven`{:class="block3motion"} en `ga naar de startpositie`{: class="block3motion"}.

--- /hint --- --- hint --- Dit zijn de codeblokken die je nodig hebt: ![boot-sprite](images/boat_resize.png)

```blocks3
if <touching color [ ] ?> then
end

go to x: (-190) y: (-150)

switch costume to (raak v)

point in direction (0)

switch costume to (normaal v)

say [Neeeeeee!] for (2) seconds
```

--- /hint --- --- hint --- Zo zou je code er uit moeten zien: ![boot-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
end
if <touching color [#663b00] ?> then
switch costume to (raak v)
say [Neeeeee!] for (2) seconds
switch costume to (normaal v)
point in direction (0)
go to x: (-190) y: (-150)
end
```

--- /hint ------ /hints ---

--- /task ---

--- task ---

Je moet ook code toevoegen die ervoor te zorgt dat je boot-sprite altijd begint met een 'normaal' uiterlijk.

Test je code opnieuw. Als je nu probeert om de boot door een houten barrière te varen moet de boot crashen en weer naar de startpositie terugkeren.

![screenshot](images/boat-crash.png)

--- /task ---