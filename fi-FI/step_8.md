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

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![portti](images/gate.png)

```blocks3
ikuisesti
päätä

käännä cw (1) astetta

kun lippu napsautetaan
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

```blocks3
kun lippu napsautti
ikuisesti
kierros cw (1) astetta
päätä
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---