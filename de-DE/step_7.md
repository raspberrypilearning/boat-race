## Hinzufügen eines Timers

Fügen wir eine Stoppuhr zu deinem Spiel hinzu, sodass der Spieler die Insel unten links so schnell wie möglich erreichen muss.

\--- task \---

Erstelle eine neue Variable namens `Zeit`{:class='block3variable'}.

![screenshot](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Du kannst die Anzeige der Variable Zeit anschalten und die Anzeige der Variablen an jede stelle der Bühne verschieben. Verschiebe die Anzeige nach unten rechts wenn du willst.

\--- /task \---

\--- task \---

Jetzt wähle Code für deine Bühne aus, damit die Stoppuhr die Zeit misst, bis das Boot die einsame Insel erreicht.

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
ändere [Zeit v] um (0.1)

Wenn grüne Flagge angecklickt wird

wiederhole fortlaufend
ende

warte (0.1) Sekunden

setze [Zeit v] auf [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
Wenn grüne Flagge angeklickt wird
setze [Zeit v] auf [0]
wiederhole fortlaufend
warte (0.1) Sekunden
ändere [Zeit v] um (0.1)
ende
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---