## Xocar!

De moment, la icona del vaixell només pot navegar per les barreres de fusta! Ara ho arreglaràs.

--- task ---

Necessitaràs dos vestuaris per al teu vaixell, un de normal i un per quan el vaixell s'estavella. Duplica el vestuari del vaixell i anomena a un "normal" i a l'altre "destrossat".

--- /task ---

--- task ---

Fes clic al vestit 'destrossat' i fes servir l'eina **Selecciona** per agafar trossos del vestit, moure'ls i fer-los girar per fer que el vaixell sembli que s'ha estavellat.

![screenshot](images/boat-hit-costume-annotated.png)

--- /task ---

--- task ---

Ara afegeix codi al teu vaixell perquè xoqui i es trenqui quan toca els trossos de fusta marró.

--- hints --- --- hint ---

Necessites afegir blocs de codi dins del teu bucle `infinitament`{:class="block3control"} de manera que el teu codi comprovi si la icona del vaixell s'ha estavellat i, si s'ha estavellat, el codi ha de restablir la posició de la icona del vaixell.

`si`{:class="block3control"} el vaixell `toca`{:class="block3sensing"} el color marró de la fusta, has de `canviar al vestit destrossat`{:class="block3looks"}, `dir Noooo! durant 2 segons`{:class="block3looks"}, i després `torna al vestit normal`{:class="block3looks"}. Finalment, necessitaràs `apuntar cap amunt`{:class="block3motion"} i `anar a la posició inicial`{:class="block3motion"}.

--- /hint --- --- hint ---

Aquí tens els blocs que necessites:

![icona-vaixell](images/boat_resize.png)

```blocks3
if <touching color [ ] ?> then
end

go to x: (-190) y: (-150)

switch costume to (destrossat v)

point in direction (0)

switch costume to (normal v)

say [Noooooo!] for (2) seconds
```

--- /hint --- --- hint ---

Així és com s'hauria de veure el teu codi:

![icona-vaixell](images/boat_resize.png)

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
switch costume to (destrossat v)
say [Noooooo!] for (2) seconds
switch costume to (normal v)
point in direction (0)
go to x: (-190) y: (-150)
end
```

--- /hint --- --- /hints ---

--- /task ---

--- task ---

També hauràs d'afegir codi per assegurar-te que el teu vaixell sempre comenci amb una aparença "normal".

Prova de nou el teu codi. Si ara intentes navegar el vaixell a través d'una barrera de fusta, el vaixell ha de xocar, destrossar-se i després tornar a la seva posició inicial.

![captura de pantalla](images/boat-crash.png)

--- /task ---