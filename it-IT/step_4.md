## Ci stiamo schiantando!

Al momento, lo sprite della barca può navigare attraverso le barriere di legno! Ora lo sistemerai.

--- task ---

Avrai bisogno di due costumi per la tua barca, un costume normale e uno per quando la barca si schianta. Duplica il costume della barca e rinomina uno dei due costumi "normale", e l'altro "colpito".

--- /task ---

--- task ---

Clicca sul costume 'colpito' e usa lo strumento **Seleziona** per catturare i pezzi del costume; spostali e ruotali per far apparire come se la barca fosse andata in pezzi.

![schermata](images/boat-hit-costume-annotated.png)

--- /task ---

--- task ---

Ora aggiungi del codice alla tua barca per far sì che si schianti e si rompa quando tocca il legno.

--- hints --- --- hint ---

È necessario aggiungere blocchi di codice all'interno del ciclo `per sempre`{:class="block3control"} in modo che il tuo codice continui a controllare se lo sprite della barca si è schiantato, ed in questo caso il codice deve reimpostare la posizione dello sprite della barca.

`se`{:class="block3control"} la barca `tocca`{:class="block3sensing"} il colore marrone del legno, devi `passare al costume colpito`{:class="block3looks"}, e ` dire Noooo! per 2 secondi` {:class="block3looks"}, quindi `torna al costume normale`{:class="block3looks"}. Infine, dovrai `puntare verso l'alto`{:class="block3motion"} e `tornare alla posizione iniziale`{:class="block3motion"}.

--- /hint --- --- hint ---

Ecco i blocchi di codice che ti serviranno:

![sprite barca](images/boat_resize.png)

```blocks3
if <touching color [ ] ?> then
end

go to x: (-190) y: (-150)

switch costume to (colpito v)

point in direction (0)

switch costume to (normale v)

say [Noooooo!] for (2) seconds
```

--- /hint --- --- hint ---

Ecco come dovrebbe apparire il risultato:

![sprite barca](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
end
if <touching color [#663b00] ?> then
switch costume to (hit v)
say [Noooooo!] for (2) seconds
switch costume to (normale v)
point in direction (0)
go to x: (-190) y: (-150)
end
```

--- /hint --- --- /hints ---

--- /task ---

--- task ---

Dovresti inoltre assicurarti che la tua barca all'inizio abbia sempre un aspetto 'normale'.

Prova di nuovo il tuo codice. Se tenti di attraversare una barriera di legno ora, la barca dovrebbe schiantarsi e poi tornare alla sua posizione di partenza.

![schermata](images/boat-crash.png)

--- /task ---