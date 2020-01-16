## Obstakels en versnellers

Op dit moment is dit spel **veel** te gemakkelijk - laten we dingen toevoegen om het interessanter te maken.

Eerst voeg je een aantal versterkers toe om de boot te versnellen.

\--- task \---

Bewerk je achtergrond door enkele witte versterkerpijlen toe te voegen.

![screenshot](images/boat-boost.png)

\--- /task \---

\--- task \---

Voeg nu extra code blokken aan de `herhaal`{:class="block3control"} lus van je boot toe zodat de boot-sprite drie extra stappen maakt wanneer het een witte pijl raakt.

![boat-sprite](images/boat_resize.png)

```blocks3
als <touching color [#FFFFFF] ?> dan
neem (3) stappen
end
```

\--- /task \---

\--- task \---

Test your game to see whether your new booster arrows speed up the boat.

\--- /task \---

Next you'll add a spinning gate that the boat has to avoid.

\--- task \---

Add a new sprite that looks like this, and call it 'gate':

![screenshot](images/boat-gate.png)

Make sure that the colour of the gate sprite is the same as the colour of the wooden barriers.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \---

Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![gate](images/gate.png)

```blocks3
herhaal
end

draai naar rechts (1) graden 

wanneer op groene vlag wordt geklikt
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
wanneer op groene vlag wordt geklikt
herhaal 
draai naar rechts (1) graden
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---