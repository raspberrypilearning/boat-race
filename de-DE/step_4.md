## Einen Unfall bauen!

Im Moment kann dein Boot einfach durch die hölzernen Hindernisse segeln! Reparieren wir das.

\--- task \---

Du brauchst zwei Kostüme für dein Boot, ein normales Kostüm und eins, wenn das Boot einen Unfall hat. Dupliziere dein Bootskostüm und nenne ein Kostüm "normal" und das andere "Unfall".

\--- /task \---

\--- task \---

Klicke auf das "**Unfall**" -Kostüm und wähle den Befehlen **Auswählen** aus, um Teile des Kostüms zu ergreifen, zu bewegen und zu drehen. Das Boot soll am Ende total kaputt aussehen.

![Screenshot](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Jetzt füge deinem Boot neuen Code hinzu, so dass es auseinander bricht, sobald es braune Holzteile berührt.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
falls <touching color [ ] ?> dann
ende

gehe zu x: (-190) y: (-150)

wechsle zu Kostüm (Unfall v)

setze Richtung auf (0) Grad

wechsle zu Kostüm (normal v)

sage [Oh nein!] für (2) Sekunden
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
Wenn grüne Flagge angeklickt wird
setze Richtung auf (0) Grad
gehe zu x: (-190) y: (-150)
wiederhole fortlaufend
wenn <(Entfernung von (Mauszeiger v)) > [5]> dann
drehe dich zu (Mauszeiger v)
gehe (1) er Schritt
ende
wenn <touching color [#663b00] ?> dann
wechsle zu Kostüm (Unfall v)
sage [Oh nein!] für (2) Sekunden
wechsle zu Kostüm (normal v)
setze Richtung auf (0) Grad
geh zu x: (-190) y: (-150)
ende
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---