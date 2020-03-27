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

Sullo stage, ` quando si fa clic sulla bandiera verde ` {: class = "block3control"}, ` imposta l'ora su 0 ` {: Class = "block3variables"}. Dentro il tuo ciclo ` per sempre ` {: class = "block3control"}, dovrai prima ` attendere 0.1 secondi ` {: class = "block3control"}, quindi ` modifica il tempo di 0.1 ` {: Class = "block3variables"}.

\--- /hint \--- \--- hint \---

Ecco i blocchi di codice che ti serviranno:

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

Ecco come dovrebbe apparire il tuo nuovo codice:

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

Ecco fatto! Prova il tuo gioco e scopri quanto velocemente riesci a raggiungere l'isola deserta!

![schermata](images/boat-variable-test.png)

\--- /task \---