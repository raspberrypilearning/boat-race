## Obstacles i potenciadors

Ara mateix aquest joc és **massa** fàcil - per això afegirem algunes coses perquè sigui més interessant.

Primer, afegiràs alguns potenciadors per accelerar el vaixell.

\--- task \---

Edita el fons del teu escenari afegint algunes fletxes potenciadores de color blanc.

![screenshot](imatges / boat-boost.png)

\--- /task \---

\--- task \---

Ara afegeix més blocs de codi al bucle ` infinitament` {: class = "block3control"} del teu vaixell de manera que l'sprite del vaixell avança tres passos addicionals quan toca una fletxa blanca. ![boat-sprite](images / boat_race_demo.png)

```blocks3
si <touching color [#FFFFFF] ?> llavors
avançar (3) passos
 finalitzar
```

\--- /task \---

\--- task \---

Prova el teu joc per veure si les noves fletxes potenciadores acceleren el vaixell.

\--- /task \---

A continuació, afegiràs una porta giratòria que el vaixell ha d’evitar.

\--- task \---

Afegeix un sprite nou que s’assembli a una porta giratòria i l'anomenes "porta":

![screenshot](imatges / boat-gate.png)

Assegura't que el color de la porta sigui el mateix que el de les barreres de fusta.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![porta](imatges / gate.png)

```blocks3
infinitament
final

gira (1) graus cw

quan es fa clic a la bandera
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

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