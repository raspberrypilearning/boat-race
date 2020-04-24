## Ostacoli e potenziamenti

Al momento, questo gioco è **troppo** facile: aggiungiamo qualcosina per renderlo più interessante.

In primo luogo, aggiungerai alcuni potenziamenti per accelerare la barca.

--- task ---

Modifica lo sfondo del progetto aggiungendo alcune frecce bianche di potenziamento.

![schermata](images/boat-boost.png)

--- /task ---

--- task ---

Ora aggiungi altri blocchi di codice al ciclo `per sempre`{:class="block3control"} in modo che lo sprite della barca si muova di tre passaggi aggiuntivi quando tocca una freccia bianca.

![sprite barca](images/boat_resize.png)

```blocks3
if <touching color [#FFFFFF] ?> then
move (3) steps
end
```

--- /task ---

--- task ---

Prova il tuo gioco per vedere se le nuove frecce bianche velocizzano la barca.

--- /task ---

Successivamente aggiungerai un cancello girevole che la barca deve evitare.

--- task ---

Aggiungi un nuovo sprite simile a questo e chiamalo 'gate':

![schermata](images/boat-gate.png)

Assicurati che il colore del cancello sia uguale a quello delle barriere di legno.

![schermata](images/brown-hsv.png)

--- /task ---

--- task ---

Assicurati che il centro dello sprite del cancello sia posizionato nel mezzo.

![schermata](images/boat-center.png)

--- /task ---

--- task ---

Aggiungi dei codici al tuo cancello per far sì che giri lentamente all'infinito.

--- hints --- --- hint ---

Aggiungi blocchi di codice allo sprite del gate in modo che `giri di 1 grado`{:class="block3motion"} `per sempre`{:class="block3control"}.

--- /hint --- --- hint ---

Ecco i blocchi di codice che ti serviranno:

![cancello](images/gate.png)

```blocks3
forever
end

turn cw (1) degrees

when flag clicked
```

--- /hint --- --- hint ---

Ecco come dovrebbe apparire il tuo nuovo codice:

![cancello](images/gate.png)

```blocks3
when flag clicked
forever
turn cw (1) degrees
end
```

--- /hint --- --- /hints ---

--- /task ---

--- task ---

Prova di nuovo il tuo gioco. Ora dovresti avere un cancello rotante che ti serve per far girare la barca.

![schermata](images/boat-gate-test.png)

--- /task ---