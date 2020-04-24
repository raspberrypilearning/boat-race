## Vittoria!

--- task ---

Ora aggiungi un altro `se`{:class="block3control"} al codice dello sprite della tua barca in modo che il giocatore vinca quando fa arrivare la barca sull'isola gialla.

Quando la barca raggiunge l'isola deserta, il gioco dovrebbe dire 'Evvai!' e interrompersi.

--- hints --- --- hint ---

Devi aggiungere più blocchi di codice all'interno del ciclo `per sempre`{:class="block3control"} in modo che il tuo codice continui a controllare se il giocatore ha vinto:

`Se`{:class="block3control"} la barca sta `toccando`{:class="block3sensitive"} il colore dell'isola, devi `dire 'Evvai!' per 2 secondi`{:class="block3look"} e poi `ferma tutto`{:class="block3control"} per terminare il gioco.

--- /hint --- --- hint ---

Ecco i blocchi di codice che ti serviranno:

![sprite barca](images/boat_resize.png)

```blocks3
say [Evvai!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

--- /hint --- --- hint ---

Ecco come dovrebbe apparire il risultato:

![sprite barca](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [Evvai!] for (2) seconds
stop [all v]
end
```

Non dimenticare che questo nuovo codice deve essere all'interno di un ciclo `per sempre`{:class="block3control"}.

--- /hint --- --- /hints --- --- /task ---