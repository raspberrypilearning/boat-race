## Botsen!

Op dit moment kan de boot-sprite gewoon door de houten barrières varen! Je gaat dat nu repareren.

\--- task \---

Je hebt twee uiterlijken voor je boot nodig, een normaal uiterlijk en een voor wanneer de boot crasht. Maak een kopie van het huidige uiterlijk en noem één uiterlijk 'normaal' en de andere 'raak'.

\--- /task \---

\--- task \---

Klik op je 'raak'-uiterlijk en gebruik het **Selectie** hulpmiddel om stukjes van de boot te pakken en deze vervolgens te verplaatsen en te draaien zodat het lijkt dat de boot in stukken is gevallen.

![screenshot](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Voeg nu code aan je boot toe zodat deze crasht en uit elkaar valt wanneer deze de bruine houten hindernis raakt.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
als <touching color [ ] ?> dan
einde

ga naar x: (-190) y: (-150)

verander uiterlijk naar (raak v)

richt naar (0) graden

verander uiterlijk naar (normaal v)

zeg [Neeeeeee! ] (2) sec.
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

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

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---