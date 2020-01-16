## Obstacles i potenciadors

Ara mateix aquest joc és **massa** fàcil - per això afegirem algunes coses perquè sigui més interessant.

Primer, afegiràs alguns potenciadors per accelerar el vaixell.

\--- task \---

Edita el fons del teu escenari afegint algunes fletxes potenciadores de color blanc.

![screenshot](imatges / boat-boost.png)

\--- /task \---

\--- task \---

Ara afegeix més blocs de codi al bucle ` infinitament` {: class = "block3control"} del teu vaixell de manera que l'sprite del vaixell avança tres passos addicionals quan toca una fletxa blanca.

![boat-sprite](images/boat_resize.png)

```blocks3
si <touching color [#FFFFFF] ?> llavors
avançar (3) passos
 finalitzar
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
infinitament
final

gira (1) graus cw

quan es fa clic a la bandera
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
quan es fa clic a la bandera
infinitament
girar (1) graus cw
final
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---