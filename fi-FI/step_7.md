## Ajastimen lisääminen

Nyt lisäät ajastimen peliin, jotta pelaaja joutuu saamaan saaren mahdollisimman nopeasti.

\--- tehtävä \---

Lisää uusi muuttuja nimeltä `time`{: class = "block3variables"} vaiheesi.

![kuvakaappaus](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Voit myös valita ajastimen haun muuttamalla uuden muuttujan näyttämistä.

\--- / tehtävä \---

\--- tehtävä \---

Lisää nyt koodilohkoja vaiheesi niin, että ajastin laskee, kunnes vene saapuu saarelle.

\--- hints \--- \--- vihje \--- Vaiheessa `kun vihreää lippua napsautetaan`{: class = "block3control"}, `aseta aika arvoon 0`{: class = "block3variables "}. `ikuisesti`{: class = "block3control"} -silmukassa sinun täytyy ensin `odottaa 0,1 sekuntia`{: class = "block3control"}, sitten `muuttaa aikaa 0,1`{: class = "block3variables" }. \--- / vihje \--- \--- vihje \--- Tässä tarvitaan koodilohkoja: ![vaihe](images/stage.png)

```blocks3
vaihda [aika v] (0,1)

kun lippu napsautti

ikuisesti
loppuun

odota (0,1) sekuntia

asetettu [aika v] - [0]
```

\--- / vihje \--- \--- vihje \--- Tässä on uusi koodisi: ![vaihe](images/stage.png)

```blocks3
kun lippu napsautti
asetusta [aika v] [0]
ikuisesti
odota (0,1) sekuntia
muutos [aika v] (0.1)
loppuun
```

\--- / vihje \--- \--- / vihjeitä \---

\--- / tehtävä \---

\--- tehtävä \---

Testaa peliäsi ja katso kuinka nopeasti saat veneen saarelle!

![kuvakaappaus](images/boat-variable-test.png)

\--- / tehtävä \---