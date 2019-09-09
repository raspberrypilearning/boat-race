## Ostacoli e potenziamenti

Al momento, questo gioco è **troppo** facile: aggiungiamo qualcosina per renderlo più interessante.

In primo luogo, aggiungerai alcuni potenziamenti per accelerare la barca.

\--- task \---

Modifica lo sfondo del progetto aggiungendo alcune frecce bianche di potenziamento.

![schermata](images/boat-boost.png)

\--- /task \---

\--- task \---

Ora aggiungi altri blocchi di codice al ciclo `forever`{: class = "block3control"} in modo che lo sprite della barca si muova di tre passaggi aggiuntivi quando tocca una freccia bianca. ![sprite barca](images / boat_race_demo.png)

```blocks3
if <touching color [#FFFFFF] ?> then
move (3) steps
end
```

\--- /task \---

\--- task \---

Prova il tuo gioco per vedere se le nuove frecce bianche velocizzano la barca.

\--- /task \---

Poi aggiungerai un cancello rotante che la barca deve evitare.

\--- task \---

Aggiungi un nuovo sprite simile a questo e chiamalo 'gate':

![schermata](images/boat-gate.png)

Assicurati che il colore del cancello sia uguale a quello delle barriere di legno.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![cancello](images/gate.png)

```blocks3
forever
end

turn cw (1) degrees

when flag clicked
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

```blocks3
when flag clicked
forever
turn cw (1) degrees
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---