## De boot besturen

De speler zal de boot-sprite met de muis bedienen.

--- task --- 

Voeg code toe aan de boot-sprite, zodat deze begint in de linkerbenedenhoek, naar boven wijzend en vervolgens de muisaanwijzer volgt.

![boot-sprite](images/boat_resize.png)

```blocks3
wanneer op groene vlag wordt geklikt
richt naar (0) graden
ga naar x: (-190) y: (-150)
herhaal
richt naar (muisaanwijzer v)
neem (1) stappen
```

--- /task ---

--- task ---

**Test je code** door op de groene vlag te klikken en de muis te verplaatsen. Beweegt de boot-sprite in de richting van de muisaanwijzer?

![screenshot](images/boat-mouse.png)

--- no-print ---

![screenshot](images/boat-pointer-test-anim.gif) 

--- /no-print ---

--- print-only --- 

![screenshot](images/boat-pointer-test-anim.png) 

--- /print-only ---

--- /task ---

--- task ---

Wat gebeurt er als de boot de muisaanwijzer bereikt? Probeer het uit om te zien wat het probleem is.

--- /task ---

--- task ---

Als je wilt voorkomen dat dit gebeurt, moet je een `als`{:class="block3control"} blok aan je code toevoegen, zodat de boot alleen beweegt als deze zich op meer dan 5 pixels afstand van de muisaanwijzer bevindt.

--- hints ---
 --- hint --- De boot mag alleen naar de muisaanwijzer wijzen en bewegen `als>`{:class="block3control"} de `afstand tot muisaanwijzer`{:class="block3sensing"} `groter dan 5 pixels`{:class="block3operators"} is.
--- /hint ---
 --- hint --- 
 
Dit zijn de code blokken die je moet toevoegen aan de code voor de boot-sprite: 

![boot-sprite](images/boat_resize.png)

```blocks3
als < [ ] > [ ] > dan

(afstand tot (muisaanwijzer v))
```

--- /hint --- 
--- hint --- 

Zo zou je nieuwe code er uit moeten zien: 

![boot-sprite](images/boat_resize.png)

```blocks3
wanneer op groene vlag wordt geklikt
richt naar (0) graden
ga naar x: (-190) y: (-150)
herhaal
als <(afstand tot (muisaanwijzer v)) > [5]> dan
richt naar (muisaanwijzer v)
neem (1) stappen
```

--- /hint ---
--- /hints ---

--- /task ---

--- task ---

Test je code opnieuw om te controleren of het probleem is opgelost.

--- /task ---