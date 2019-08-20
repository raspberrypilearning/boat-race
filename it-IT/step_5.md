## Vittoria!

\--- task \--- Ora aggiungi un'altra dichiarazione `if` {: class = "block3control"} al codice dello sprite della tua barca in modo che il giocatore vince quando fa arrivare la barca all'isola gialla.

Quando la barca raggiunge l'isola deserta, il gioco dovrebbe dire 'Evvai!' e interrompersi.

\--- hints \--- \--- hint \--- Devi aggiungere del codice all'interno del blocco `forever` per far sì che il codice continui a controllare se il giocatore ha vinto:

`Se`{:class="block3control"} la barca sta `toccando`{:class="block3sensitive"} il colore dell'isola, devi `dire 'Evvai!' per 2 secondi`{:class="block3look"} e poi `stop all`{:class="block3control"} per terminare il gioco. \--- /hint \--- \--- hint \--- Qui ci sono i blocchi di codice che ti serviranno: ![boat-sprite](images/boat_resize.png)

```blocks3
say [Evvai!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

\--- /hint \--- \--- hint \--- Ecco come dovrebbe apparire il tuo codice: ![boat-sprite](images / boat_race_demo.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [Evvai!] for (2) seconds
stop [all v]
end
```

Non dimenticare che questo nuovo codice deve essere dentro `forever`{:class="block3control"}. -- /hint \--- -- /hints \--- \--- /task \---