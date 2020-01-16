## Afegir un temporitzador

Ara afegiràs un cronòmetre al teu joc, de manera que el jugador ha d'arribar a l'illa el més ràpidament possible.

\--- task \---

Afegeix una nova variable al teu escenari i anomenala `temps`{:class = "blockvariable"}.

![screenshot](images / boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

També pots triar un aspecte del teu temporitzador canviant la manera de mostrar la vostra nova variable.

\--- /task \---

\--- task \---

Ara afegeix el codi al teu escenari perquè el temporitzador estigui comptant fins que el vaixell arribi a l'illa deserta.

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
canviar [temps v] per (0.1)

quan es fa clic a la bandera

infinitament
fi

espera (0,1) segons

reiniciar [temps v] a [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
quan es fa clic a la bandera
posar [temps v] a [0]
infinitament
esperar (0,1) segons
canviar [temps v] per (0.1)
fi
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---