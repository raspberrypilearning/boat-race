## Esteet ja vahvistimet

Juuri nyt peli on **** liian helppoa, joten lisäät jotain mielenkiintoisemmaksi.

Ensinnäkin voit lisätä joitakin vahvistimia nopeuttaaksesi venettä.

\--- tehtävä \---

Muokkaa vaiheesi taustaa lisäämällä joitakin valkoisia tehostusnuolia.

![kuvakaappaus](images/boat-boost.png)

\--- /task \---

\--- task \---

Lisää nyt lisää koodilohkoja veneen `ikuisesti`{: class = "block3control"} silmukkaan niin, että veneen sprite siirtää kolme ylimääräistä vaihetta, kun se koskettaa valkoista nuolta. ![veneen-sprite](images/boat_resize.png)

```blocks3
jos <touching color [#FFFFFF] ?> sitten
liikkua (3) vaiheet
loppuun
```

\--- / tehtävä \---

\--- tehtävä \---

Testaa peliäsi nähdäksesi, onko uudet tehostusnuolet nopeuttaneet venettä.

\--- / tehtävä \---

Seuraavaksi lisätään pyörivä portti, jonka veneellä on vältettävä.

\--- tehtävä \---

Lisää uusi sprite, joka näyttää tältä, ja kutsu sitä "portiksi":

![kuvakaappaus](images/boat-gate.png)

Varmista, että portin spriitin väri on sama kuin puupalkkien väri.

\--- / tehtävä \---

\--- tehtävä \---

Varmista, että portin spriitin keskipiste on keskellä.

![kuvakaappaus](images/boat-center.png)

\--- / tehtävä \---

\--- tehtävä \---

Lisää koodi portti sprite jotta se spin hitaasti ikuisesti.

\--- hints \--- \--- vihje \--- Lisää koodilohkot portin spriteille niin, että se `muuttuu 1 asteen`{: class = "block3motion"} `ikuisesti`{: class = "block3control"} . \--- / vihje \--- \--- vihje \--- Tässä on tarvitsemasi koodilohkot: ![portti](images/gate.png)

```blocks3
ikuisesti
päätä

käännä cw (1) astetta

kun lippu napsautetaan
```

\--- / vihje \--- \--- vihje \--- Tässä on uusi koodisi: ![portti](images/gate.png)

```blocks3
kun lippu napsautti
ikuisesti
kierros cw (1) astetta
päätä
```

\--- / vihje \--- \--- / vihjeitä \---

\--- / tehtävä \---

\--- tehtävä \---

Testaa peli uudelleen. Sinun pitäisi nyt olla pyörivä portti, jota tarvitset sekoittamaan venettäsi.

![kuvakaappaus](images/boat-gate-test.png)

\--- / tehtävä \---