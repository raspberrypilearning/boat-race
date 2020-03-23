## De boot besturen

De speler zal de boot-sprite met de muis bedienen.

--- task --- Voeg code toe aan de boot-sprite, zodat deze begint in de linkerbenedenhoek, naar boven wijzend en vervolgens de muisaanwijzer volgt.

![boot-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
point towards (mouse-pointer v)
move (1) steps
```

--- /task ---

--- task ---

**Test je code** door op de groene vlag te klikken en de muis te verplaatsen. Beweegt de boot-sprite in de richting van de muisaanwijzer?

![schermafdruk](images/boat-mouse.png)

--- no-print --- ![screenshot](images/boat-pointer-test-anim.gif) --- /no-print ---

--- print-only --- ![screenshot](images/boat-pointer-test-anim.png) --- /print-only ---

--- /task ---

--- task ---

Wat gebeurt er als de boot de muisaanwijzer bereikt? Probeer het uit om te zien wat het probleem is.

--- /task ---

--- task ---

Als je wilt voorkomen dat dit gebeurt, moet je een `als`{:class="block3control"} blok aan je code toevoegen, zodat de boot alleen beweegt als deze zich op meer dan 5 pixels afstand van de muisaanwijzer bevindt.

--- hints ---
 --- hint --- De boot mag alleen naar de muisaanwijzer wijzen en bewegen `als>`{:class="block3control"} de `afstand tot muisaanwijzer`{:class="block3sensing"} `groter dan 5 pixels`{:class="block3operators"} is.
--- /hint ---
 --- hint --- Dit zijn de code blokken die je moet toevoegen aan de code voor de boot-sprite: ![boot-sprite](images/boat_resize.png)

```blocks3
if < [ ] > [ ] > then

(distance to (mouse-pointer v))
```

--- /hint --- --- hint --- Hier is hoe je code eruit zou moeten zien: ![boot-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

--- /hint ------ /hints ---

--- /task ---

--- task ---

Test je code opnieuw om te controleren of het probleem is opgelost.

--- /task ---
