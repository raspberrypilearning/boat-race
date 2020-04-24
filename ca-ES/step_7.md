## Afegir un temporitzador

Ara afegiràs un cronòmetre al teu joc, de manera que el jugador ha d'arribar a l'illa el més ràpid possible.

--- task ---

Afegeix una nova variable al teu escenari anomenada `temps`{:class = "block3variable"}.

![screenshot](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

També pots triar un aspecte del teu temporitzador canviant la manera de mostrar la teva nova variable.

--- /task ---

--- task ---

Ara afegeix blocs de codi al teu escenari perquè el temporitzador estigui comptant fins que el vaixell arribi a l'illa.

--- hints --- --- hint ---

A l'escenari `quan es fa clic a la bandera verda`{:class="block3control"}, `reiniciar el temps a 0`{:class="block3variables"}. Dins del teu bucle `per sempre`{:class="block3control"}, primer hauràs de `esperar 0.1 segons`{:class="block3control"}, llavors `canviar el temps a 0,1`{:class="block3variables"}.

--- /hint --- --- hint ---

Aquí tens els blocs que necessites:

![escenari](images/stage.png)

```blocks3
change [temps v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [temps v] to [0]
```

--- /hint --- --- hint ---

Així és com s'hauria de veure el teu codi:

![escenari](images/stage.png)

```blocks3
when flag clicked
set [temps v] to [0]
forever
wait (0.1) seconds
change [temps v] by (0.1)
end
```

--- /hint --- --- /hints ---

--- /task ---

--- task ---

Prova el joc i vejam com de ràpid aconsegueixes arribar a l'illa!

![captura de pantalla](images/boat-variable-test.png)

--- /task ---