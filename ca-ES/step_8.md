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

\--- /task \---

\--- task \---

Assegura't que el centre de l'sprite de la porta està situat al mig d'aquest.

![screenshot](imatges / boat-center.png)

\--- /task \---

\--- task \---

Afegeix codi a la teva porta perquè giri lentament de manera infinita.

\--- hints \--- \--- hint \--- Afegeix blocs de codi l'sprite de la porta de manera que ` gira 1 grau ` {: class = "block3motion"} ` per sempre ` {: class = "block3control"}. \--- /hint \--- \--- hint \--- Aquí tens els blocs de codi que necessites: ![porta](imatges / gate.png)

```blocks3
infinitament
final

gira (1) graus cw

quan es fa clic a la bandera
```

\--- /hint \--- \--- hint \--- Això és el que hauria de tenir el teu codi: ![porta](imatges / gate.png)

```blocks3
quan es fa clic a la bandera
infinitament
girar (1) graus cw
final
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Prova el vostre joc de nou. Ara hauries de tenir una porta giratòria que necessites per remoure el vaixell.

![screenshot](images/boat-gate-test.png)

\--- /task \---