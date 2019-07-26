## Voittaa!

\--- tehtävä \--- Lisää vielä `jos`{: class = "block3control"} lausunto veneen sprite-koodiin niin, että pelaaja voittaa, kun veneen saapuu keltaiselle saarelle.

Kun vene saapuu saarelle, pelin pitäisi sanoa "YEAH!", Ja sitten sen pitäisi päättyä.

\--- hints \--- \--- vihje \--- Sinun täytyy lisätä lisää koodilohkoja `ikuisesti`{: class = "block3control"} silmukkaan niin, että koodisi tarkistaa, onko pelaaja voittanut:

`jos`{: class = "block3control"} vene on `koskettaa`{: class = "block3sensing"} saaren väriä, sinun täytyy `sanoa 'YEAH!' 2 sekuntia`{: class = "block3looks"} ja sitten `lopettaa kaikki`{: class = "block3control"} lopettaaksesi pelin. \--- / vihje \--- \--- vihje \--- Tässä on tarvitsemasi koodilohkot: ![veneen-sprite](images/boat_resize.png)

```blocks3
sano [YEAH!] (2) sekunnin ajan

jos <touching color [#FFFF99] ?> sitten
pää

lopeta [kaikki v]

```

\--- / vihje \--- \--- vihje \--- Tässä on uusi koodisi: ![veneen-sprite](images/boat_resize.png)

```blocks3
jos <touching color [#FFFF99] ?> sitten
sanoa [YEAH!] (2) sekunnin ajan
pysäytys [kaikki v]
pää
```

Älä unohda, että tämän uuden koodin täytyy olla `ikuisesti`{: class = "block3control"} -silmukassa. \--- / vihje \--- \--- / vihjeitä \--- \--- / tehtävä \---