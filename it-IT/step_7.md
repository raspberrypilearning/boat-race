## Aggiungere un timer

Aggiungiamo un timer al tuo gioco, per far sì che il giocatore debba raggiungere l'isola deserta il più velocemente possibile.

\--- task \---

Aggiungi una nuova variabile chiamata `time`{:class="block3variables"} al tuo progetto.

![screenshot](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Puoi anche scegliere un look per il tuo timer cambiando il modo in cui viene visualizzata la nuova variabile.

\--- /task \---

\--- task \---

Ora aggiungi blocchi di codice al tuo progetto in modo che il timer esegua il conteggio fino a quando la barca raggiunge l'isola.

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
change [time v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [time v] to [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

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