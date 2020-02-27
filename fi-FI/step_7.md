## Ajastimen lisääminen

Lisätään peliin ajastin, joten pelaajan on päästävä saarelle niin pian kuin mahdollista.

--- task ---

Lisää uusi muuttuja nimeltä `aika`{:class="block3variables"} Esiintymislavallesi.

![kuvakaappaus](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Voit myös valita ajastimen ulkoasun muuttamalla uuden muuttujan näyttötapaa.

--- /task ---

--- task ---

Lisää koodilohkoja esiintymislavallesi niin, että aika kasvaa, kunnes vene saapuu saarelle.

--- hints --- --- hint ---

Esiintymislavalla, `kun vihreää lippua klikataan`{:class="block3control"}, `aseta aika arvoon 0`{:class="block3variables"}. `ikuisesti`{:class="block3control"} -silmukan sisällä sinun täytyy ensin `odottaa 0.1 sekuntia`{:class="block3control"}, sitten `muuttaa aikaa 0.1:llä`{:class="block3variables"}.

--- /hint --- --- hint ---

Tässä on tarvitsemasi koodilohkot:

![esiintymislava](images/stage.png)

```blocks3
lisää muuttujaan [aika v] arvo (0.1)

kun klikataan lippua

ikuisesti
end

odota (0.1) sekuntia

aseta [aika v] arvoon [0]
```

--- /hint --- --- hint ---

Uuden koodisi tulisi näyttää seuraavalta:

![esiintymislava](images/stage.png)

```blocks3
kun klikataan lippua
aseta [aika v] arvoon [0]
ikuisesti 
 odota (0.1) sekuntia
 lisää muuttujaan [aika v] arvo (0.1)
end
```

--- /hint --- --- /hints ---

--- /task ---

--- task ---

Testaa peliä ja kokeile kuinka nopeasti pääset saarelle!

![kuvakaappaus](images/boat-variable-test.png)

--- /task ---