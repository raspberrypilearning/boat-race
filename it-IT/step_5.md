## Ci stiamo schiantando

\--- task \--- Ora aggiungi un altra dichiarazione `if` {: class = "block3control"} al codice dello sprite della tua barca in modo che il giocatore vince quando fa arrivare la barca all'isola gialla.

Quando la barca raggiunge l'isola deserta, il gioco dovrebbe dire 'Evvai!' e interrompersi.

\--- hints \--- \--- hint \--- Devi aggiungere del codice all'interno del blocco `forever` per far sì che il codice continui a controllare se il giocatore ha vinto:

`se` la barca `tocca` il colore dell'isola del tesoro, devi `dire 'YEAH!' per 2 secondi` e poi `fermare` il gioco. \--- /hint \--- \--- hint \--- Qui ci sono i blocchi di codice che ti serviranno: ![boat-sprite](images/boat_resize.png)

```blocks3
say [YEAH!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

\--- /hint \--- \--- hint \--- Ecco come dovrebbe apparire il tuo codice: ![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
```

Non dimenticare che questo nuovo codice deve essere dentro `forever`{:class="block3control"}. -- /hint \--- -- /hints \--- \--- /task \---