## Winning!

\--- task \--- Ara afegeix un altre declaració de ` si ` {: class = "block3control"} al codi de l' sprite del vaixell perquè el jugador guanyi quan el vaixell arriba a la illa groga.

Quan el vaixell arriba a l'illa, el joc hauria de dir 'YEAH!' i a continuació hauria d'acabar-se.

\--- hints \--- \--- hint \--- Necessites afegir més codi al teu bucle`infinitament` perquè el teu codi controli si el jugador ha guanyat:

`si` {:class="block3control"} el vaixell està `tocant` el color de l'illa, has de `dir 'YEAH!' durant 2 segons` i després `parar tot` {:class="block3control"} per finalitzar el joc. \--- /hint \--- \--- hint \--- Hi ha dos conjunts de blocs de codi que pots utilitzar: ![boat-sprite](images / boat_race_demo.png)

```blocks3
dir [YEAH!] durant (2) segons

si <touching color [#FFFF99] ?> llavors
parar

parar [all v]

```

\--- /hint \--- \--- hint \--- Això és el que hauria de tenir el teu codi: ![boat-sprite](images / boat_race_demo.png)

```blocks3
si <touching color [#FFFF99] ?> llavors
dir [YEAH!] durant (2) segons
parar [all v]
fi
```

No t'oblidis que aquest nou codi ha d’estar dins del bucle `infinitament ` {: class = "block3control"}. \--- / pista \--- \--- / consells \--- \--- / tasca \---