## Kaatuu!

Tällä hetkellä veneen sprite voi yksinkertaisesti purjehtia puisten esteiden läpi! Aiot korjata sen nyt.

\--- tehtävä \---

Sinun tarvitsee kaksi pukua veneesi sprite: yksi normaali puku, ja yksi kun vene kaatuu. Kopioi veneen sprite-puku ja anna yksi puku "normaali" ja toinen "osuma".

\--- / tehtävä \---

\--- tehtävä \---

Napsauta hittipukua ja käytä **Select** -työkalua tarttua puvun paloihin ja siirtää niitä ja kääntämällä niitä, jotta vene näyttää kaltaiselta.

![kuvakaappaus](images/boat-hit-costume-annotated.png)

\--- / tehtävä \---

\--- tehtävä \---

Nyt lisää koodi veneellesi niin, että se kaatuu ja hajoaa, kun se koskettaa ruskeat puiset esteet.

\--- hints \--- \--- vihje \--- Sinun täytyy lisätä koodilohkoja `ikuisesti`{: class = "block3control"} silmukkaan niin, että koodi tarkistaa, onko veneen sprite kaatunut, ja jos se on kaatunut, koodin on palautettava veneen sprite-asema.

`, jos`{: class = "block3control"} vene on `koskettaa`{: class = "block3sensing"} ruskea väri puun, sinun täytyy `kytkin osuma puku`{: class = "block3looks"} , `sanoo Noooo! 2 sekuntia`{: class = "block3looks"} ja sitten `palaa normaaliin puvuun`{: class = "block3looks"}. Lopuksi sinun täytyy `piste ylös`{: class = "block3motion"} ja `siirtyä alkuasentoon`{: class = "block3motion"}.

\--- / vihje \--- \--- vihje \--- Tässä on tarvitsemasi koodilohkot: ![veneen-sprite](images/boat_resize.png)

```blocks3
jos <touching color [ ] ?> sitten
pää

siirrytään x: (-190) y: (-150)

kytkinpuku (osuma v)

pisteen suuntaan (0)

kytkinpuku (normaaliin v)

sanoa [Noooooo!] (2) sekuntia
```

\--- / vihje \--- \--- vihje \--- Tässä on, mitä koodisi näyttää: ![veneen-sprite](images/boat_resize.png)

```blocks3
kun lippu napsautti
pistettä suuntaan (0)
siirry kohtaan x: (-190) y: (-150)
ikuisesti
jos <(etäisyys (hiiren osoitin v)) > [5]> ja
piste (hiiri- osoitin v)
siirtää (1) vaiheet
loppuun
jos <touching color [#663b00] ?> sitten
kytkeä puku (osuma v)
sanoa [Noooooo!] (2) sekuntia
kytke puku (normaali v)
pistettä suuntaan (0)
siirry kohtaan x: (-190) y: (-150)

```

\--- / vihje \--- \--- / vihjeitä \---

\--- /task \---

\--- task \---

Sinun pitäisi myös lisätä koodi varmistaaksesi, että veneen sprite alkaa aina etsimään "normaalia".

Testaa koodi uudelleen. Jos yrität purjehtia veneen puisen esteen läpi, veneen tulee kaatua ja sitten siirtyä takaisin lähtöasentoonsa.

![kuvakaappaus](images/boat-crash.png)

\--- / tehtävä \---