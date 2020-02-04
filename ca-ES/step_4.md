## Xocar!

De moment, la icona del vaixell només pot navegar per les barreres de fusta! Ara ho arreglaràs.

\--- task \---

Necessitaràs dos vestuaris per al teu vaixell, un de normal i un per quan el vaixell s'estavella. Duplica el vestuari del vaixell i anomena a un "normal" i a l'altre "destrossat".

\--- /task \---

\--- task \---

Fes clic al vestit 'destrossat' i fes servir l'eina ** Selecciona ** per agafar trossos del vestit, moure'ls i fer-los girar per fer que el vaixell sembli que s'ha estavellat.

![screenshot](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Ara afegeix codi al teu vaixell perquè xoqui i es trenqui quan toca els trossos de fusta marró.

\--- hints \--- \--- hint \---

Necessites afegir blocs de codi dins del teu bucle `infinitament`{:class="block3control"} de manera que el teu codi comprovi si la icona del vaixell s'ha estavellat i, si s'ha estavellat, el codi ha de restablir la posició de la icona del vaixell.

` si ` {:class = "block3control"} el vaixell `toca ` {:class = "block3sensing"} el color marró de la fusta, has de ` canviar al vestit destrossat ` {:class = "block3looks"}, ` dir Noooo! durant 2 segons ` {:class = "block3looks"}, i després ` torna al vestit normal ` {:class = "block3looks"}. Finalment, necessitaràs ` apuntar cap amunt ` {:class = "block3motion"} i ` anar a la posició inicial ` {:class = "block3motion"}.

\--- /hint \--- \--- hint \---

Aquí tens els blocs que necessites:

![icona-vaixell](images/boat_resize.png)

```blocks3
si <touching color [ ] ?> llavors
fi

anar a x: (-190) y: (-150)

canviar el vestit a (destrossat v)

apuntar en direcció (0)

canviar el vestit a (normal v)

dir [Noooooo!] durant (2) segons
```

\--- /hint \--- \--- hint \---

Així és com s'hauria de veure el teu codi:

![icona-vaixell](images/boat_resize.png)

```blocks3
quan es fa clic a la bandera
apuntar en la direcció (0)
anar a x: (-190) y: (-150)
per sempre
si <(distància del (punter del ratolí v)) > [5]> llavors,
apuntar al (punter del ratolí v)
mou (1) passos
fi
si <touching color [#663b00] ?> llavors
canviar vestit a (destrossat v)
dir [noooooo!] durant (2) segons
canviar vestit a (normal v)
apuntar en la direcció (0)
anar a x: (-190) y: (-150)
fi
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

També hauràs d'afegir codi per assegurar-te que el teu vaixell sempre comenci amb una aparença "normal".

Prova de nou el teu codi. Si ara intentes navegar el vaixell a través d'una barrera de fusta, el vaixell ha de xocar, destrossar-se i després tornar a la seva posició inicial.

![captura de pantalla](images/boat-crash.png)

\--- /task \---