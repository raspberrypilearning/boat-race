## Voittaminen!

--- task ---

Lisää vielä `jos`{:class="block3control"} lause veneen koodiin niin, että pelaaja voittaa, kun vene saapuu keltaiselle saarelle.

Kun vene saapuu saarelle, pelin pitäisi sanoa "JOO!", ja sitten sen pitäisi päättyä.

--- hints --- --- hint ---

Sinun täytyy lisätä lisää koodilohkoja `ikuisesti`{:class="block3control"} silmukan sisään niin, että koodisi tarkistaa jatkuvasti, onko pelaaja voittanut:

`jos`{:class="block3control"} vene `koskettaa`{:class="block3sensing"} saaren väriä, sinun täytyy `sanoa 'JOO!' 2 sekuntia`{:class="block3looks"} ja sitten `pysäytä kaikki`{:class="block3control"} lopettaaksesi pelin.

--- /hint --- --- hint ---

Tässä on tarvitsemasi koodilohkot:

![vene-hahmo](images/boat_resize.png)

```blocks3
sano [JOO!] (2) sekunnin ajan

jos <touching color [#FFFF99] ?>, niin
end

pysäytä [all v]

```

--- /hint --- --- hint ---

Uuden koodisi tulisi näyttää seuraavalta:

![vene-hahmo](images/boat_resize.png)

```blocks3
jos <touching color [#FFFF99] ?> , niin 
  sano [JOO!] (2) sekunnin ajan
  pysäytä [all v]
end
```

Älä unohda, että tämän uuden koodin täytyy olla `ikuisesti`{:class="block3control"} -silmukan sisällä.

--- /hint --- --- /hints --- --- /task ---