## Controllare la barca

Il giocatore controllerà lo sprite della barca con il mouse.

--- task ---

Aggiungi delle righe di codice alla tua barca per far sì che parta dell'angolo in basso a sinistra, puntando verso l'alto, e che segua il puntatore del mouse.

![sprite barca](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
point towards (mouse-pointer v)
move (1) steps
```

--- /task ---

--- task ---

**Prova il tuo codice** cliccando sulla bandiera verde e spostando il mouse. La barca si muove verso il puntatore del mouse?

![schermata](images/boat-mouse.png)

--- no-print ---

![schermata](images/boat-pointer-test-anim.gif)

--- /no-print ---

--- print-only ---

![schermata](images/boat-pointer-test-anim.png)

--- /print-only ---

--- /task ---

--- task ---

Cosa succede quando la barca raggiunge il puntatore del mouse? Prova per vedere qual è il problema.

--- /task ---

--- task ---

Per evitare che ciò accada, è necessario aggiungere un blocco `se`{:class="block3control"} al tuo codice, in modo che lo sprite della barca si sposti solo se è distante più di 5 pixel dal puntatore del mouse.

--- hints --- --- hint ---

La barca dovrebbe puntare solo verso il puntatore del mouse e spostare `se`{:class="block3control"} la distanza `dal puntatore del mouse`{:class="block3sensing"} è `maggiore di 5 pixel`{:class="block3operators"}.

--- /hint --- --- hint ---

Ecco i blocchi di codice che devi aggiungere al tuo codice dello sprite della barca:

![sprite della barca](images/boat_resize.png)

```blocks3
if < [ ] > [ ] > then

(distance to (mouse-pointer v))
```

--- /hint --- --- hint ---

Ecco come dovrebbe apparire il risultato:

![sprite della barca](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

--- /hint --- --- /hints ---

--- /task ---

--- task ---

Fai un'altra prova per vedere se il problema è stato risolto.

--- /task ---