## Veneen ohjaaminen

Pelaaja ohjaa venettä hiirellä.

\--- task \--- Lisää koodia veneeseesi niin, että se lähtee vasemmasta alakulmasta osoittaen ylöspäin ja seuraa hiiren osoitinta.

![boat-sprite](images/boat_resize.png)

```blocks3
kun klikataan
osoita suuntaan (0)
mene sijaintiin x: (-190) y: (-150)
ikuisesti 
  osoita kohti (mouse-pointer v)
  liiku (1) askelta
end
```

\--- /task \---

\--- task \---

**Testaa koodi** klikkaamalla vihreää lippua ja liikuttamalla hiirtä. Liikkuuko vene kohti hiiren osoitinta?

![screenshot](images/boat-mouse.png)

\--- no-print \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- /no-print \---

\--- print-only \--- ![screenshot](images/boat-pointer-test-anim.png) \--- /print-only \---

\--- /task \---

\--- task \---

Mitä tapahtuu, kun vene saavuttaa hiiren osoittimen? Kokeile sitä, jotta näet mikä ongelma on.

\--- /task \---

\--- task \---

Jos haluat estää tämän, sinun on lisättävä koodiisi `jos`{:class="block3control"} lohko, niin että vene liikkuu vain, jos se on enemmän kuin 5 pikselin etäisyydellä hiirestä.

\--- hints \--- \--- hint \--- Veneen pitäisi osoittaa kohti hiiren osoitinta ja liikkua vain, `jos`{:class="block3control"} `etäisyys hiiren osoittimeen`{:class="block3sensing"} on `suurempi kuin 5 pikseliä`{:class="block3operators"}. \--- /hint \--- \--- hint \--- Nämä ovat koodilohkoja, jotka sinun täytyy lisätä koodiin veneen kuvaa varten: ![boat-sprite](images/boat_resize.png)

```blocks3
jos < [ ] > [ ] > , niin
end

(etäisyys kohteeseen (mouse-pointer v))
```

\--- /hint \--- \--- hint \--- Koodisi pitäisi näyttää tältä: ![boat-sprite](images/boat_resize.png)

```blocks3
kun klikataan
osoita suuntaan (0)
mene sijaintiin x: (-190) y: (-150)
ikuisesti 
  jos <(etäisyys kohteeseen (mouse-pointer v)) > [5]> , niin 
    osoita kohti (mouse-pointer v)
    liiku (1) askelta
  end
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Testaa koodi uudelleen tarkistaaksesi, onko ongelma nyt korjattu.

\--- /task \---