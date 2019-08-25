## Hinzufügen eines Timers

Fügen wir eine Stoppuhr zu deinem Spiel hinzu. Der Spieler muss die Insel unten links so schnell wie möglich erreichen.

\--- task \---

Erstelle eine neue Variable namens `Zeit`{:class='block3variable'}.

![screenshot](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Du kannst die Anzeige der Variable Zeit anschalten und die Anzeige der Variablen an jede stelle der Bühne verschieben. Verschiebe die Anzeige nach unten rechts wenn du willst.

\--- /task \---

\--- task \---

Jetzt wähle Code für deine Bühne aus, damit die Stoppuhr die Zeit nimmt bis das Boot die einsame Insel erreicht.

\--- hints \--- \--- hint \--- On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}. \--- /hint \--- \--- hint \--- Here are the code blocks you'll need: ![stage](images/stage.png)

```blocks3
change [time v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [time v] to [0]
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![stage](images/stage.png)

```blocks3
when flag clicked
set [time v] to [0]
forever
wait (0.1) seconds
change [time v] by (0.1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---