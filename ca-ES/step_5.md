## Guanyar!

\--- task \---

Ara afegeix una altra declaració `si`{:class="block3control"} al codi de la icona del vaixell perquè el jugador guanyi quan el vaixell arribi a l'illa groga.

Quan el vaixell arriba a l'illa, el joc hauria de dir 'SIIIII!!'' i a continuació hauria d'acabar-se.

\--- hints \--- \--- hint \---

Necessites afegir més codi al teu bucle `per sempre`{:class="block3control"} perquè el teu codi controli si el jugador ha guanyat:

`si` {:class="block3control"} el vaixell està `tocant`{:class="block3sensing"} el color de l'illa, has de `dir 'SIIIIII!' durant 2 segons`{:class="block3looks"} i després `parar tot` {:class="block3control"} per finalitzar el joc.

\--- /hint \--- \--- hint \---

Aquí tens els blocs que necessites:

![icona-vaixell](images/boat_resize.png)

```blocks3
dir [SIIIIIII!] durant (2) segons

si <touching color [#FFFF99] ?> llavors
fi

parar [totes v]

```

\--- /hint \--- \--- hint \---

Així és com s'hauria de veure el teu codi:

![icona-vaixell](images/boat_resize.png)

```blocks3
si <touching color [#FFFF99] ?> llavors
dir [SIIIIII!] durant (2) segons
parar [totes v]
fi
```

No t'oblidis que aquest nou codi ha d’estar dins del bucle `per sempre`{:class="block3control"}.

\--- /hint \--- \--- /hints \--- \--- /task \---