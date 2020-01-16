## Esteet ja lisävoimat

Tällä hetkellä tämä peli on **aivan** liian helppo, joten sinä lisäät asioita, jotta se olisi mielenkiintoisempi.

Ensin, sinä lisäät lisävoimia nopeuttaaksesi venettä.

\--- task \---

Muokkaa Esiintymislavasi taustaa lisäämällä valkoisia lisävoima nuolia.

![kuvakaappaus](images/boat-boost.png)

\--- /task \---

\--- task \---

Lisää nyt lisää koodilohkoja veneen `ikuisesti`{:class="block3control"} silmukkaan niin, että vene siirtyy kolme ylimääräistä askelta, kun se koskettaa valkoista nuolta.

![boat-sprite](images/boat_resize.png)

```blocks3
jos <touching color [#FFFFFF] ?> , niin 
  liiku (3) askelta
end
```

\--- /task \---

\--- task \---

Test your game to see whether your new booster arrows speed up the boat.

\--- /task \---

Next you'll add a spinning gate that the boat has to avoid.

\--- task \---

Add a new sprite that looks like this, and call it 'gate':

![screenshot](images/boat-gate.png)

Make sure that the colour of the gate sprite is the same as the colour of the wooden barriers.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \---

Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![gate](images/gate.png)

```blocks3
ikuisesti
end

käänny ↻ (1) astetta

kun klikataan ⚑
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
kun klikataan ⚑
ikuisesti 
  käänny ↻ (1) astetta
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---