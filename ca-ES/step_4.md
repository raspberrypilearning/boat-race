## Xocar!

De moment, l’sprite del vaixell només pot navegar per les barreres de fusta! Ara ho millorarem.

\--- task \---

Necessitaràs dues disfresses per al teu vaixell, una disfressa normal i una per quan el vaixell s'estavella. Duplica la disfressa del vaixell i anomena una disfressa "normal" i l'altra "xoc".

\--- /task \---

\--- task \---

Fes clic a la disfressa "xoc" i fes servir l'eina ** Selecciona ** per agafar trossos de la disfressa, moure'ls i fer-los girar per fer que el vaixell sembli que s'ha estavellat.

![screenshot](images / boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Ara afegeix codi al teu vaixell perquè xoqui i es trenqui quan toca els trossos de fusta marró.

\--- hints \--- \--- hint \--- Necessites afegir blocs de codi dins del teu bucle `infinitament` {: class = "block3control"} de manera que el teu codi comprova si l'sprite del vaixell s'ha estavellat i, si s'ha estavellat, el codi ha de restablir la posició de l'sprite del vaixell.

` si ` {: class = "block3control"} el vaixell `toca ` {: class = "block3sensing"} el color marró de la fusta, has de ` canviar a la disfressa xoc ` {: class = "block3looks"}, ` dir Noooo! durant 2 segons ` {: class = "block3looks"}, i després ` torna a la disfressa normal ` {: class = "block3looks"}. Finalment, necessitaràs ` apuntar cap amunt ` {: class = "block3motion"} i ` anar a la posició inicial ` {: class = "block3motion"}.

\--- /hint \--- \--- hint \--- Hi ha dos conjunts de blocs de codi que pots utilitzar: ![boat-sprite](images / boat_race_demo.png)

```blocks3
si <touching color [ ] ?> llavors
fi

anar a x: (-190) y: (-150)

canviar la disfressa a (xoc v)

apuntar en direcció (0)

canviar la disfressa a (normal v)

dir [Noooooo!] durant (2) segons
```

\--- /hint \--- \--- hint \--- Això és el que hauria de tenir el teu codi: ![boat-sprite](images/boat_resize.png)

```blocks3
quan es fa clic a la bandera
apuntar en la direcció (0)
anar a x: (-190) y: (-150)
infinitament
si <(distància del (punter del ratolí v)) > [5]> llavors,
apuntar al (punter del ratolív)
avançar (1) passos
fi
si <touching color [#663b00] ?> llavors
canviar disfressa a (xoc v)
dir [noooooo!] durant (2) segons
canviar disfressa a ( normal v)
apuntar en la direcció (0)
anar a x: (-190) y: (-150)
fi
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

També hauràs d'assegurar-te que el teu vaixell sempre comenci amb una aparença "normal".

Prova de nou el teu codi. Si ara intentes navegar el vaixell a través d'una barrera de fusta, el vaixell ha de xocar i després tornar a la seva posició inicial.

![screenshot](images/boat-crash.png)

\--- /task \---