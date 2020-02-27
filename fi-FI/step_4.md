## Törmääminen!

Tällä hetkellä vene voi yksinkertaisesti purjehtia puisten esteiden läpi! Tämän sinä tulet korjaamaan nyt.

\--- task \---

Tarvitset kaksi asustetta veneellesi, yksi normaali asuste ja yksi veneen törmäykseen. Kopioi vene asuste ja nimeä ensimmäinen asuste nimellä "normaali" ja toinen "osuma".

\--- /task \---

\--- task \---

Napsauta 'osuma' -asuasi ja käytä **Valitse** työkalua tarttuaksesi pukuosiin ja siirrä ja käännä niitä, jotta näyttää siltä kuin vene olisi hajonnut kappaleiksi.

![kuvakaappaus](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Nyt, lisää koodia veneeseesi niin, että se törmää ja hajoaa, kun se koskettaa ruskeita puupaloja.

\--- hints \--- \--- hint \---

Sinun täytyy lisätä koodilohkoja `ikuisesti`{: class = "block3control"} silmukan sisään niin, että koodi tarkistaa, onko vene törmännyt, ja jos se on törmännyt, koodin on nollattava veneen sijainti.

`jos`{:class="block3control"} vene `koskettaa`{:class="block3sensing"} puun ruskeaa väriä, sinun täytyy `vaihtaa osuma asusteeseen`{:class="block3looks"}, `sano Eiiii! 2 sekuntia`{:class="block3looks"}, ja sitten `vaihda takaisin normaaliin asusteeseen`{:class="block3looks"}. Lopuksi sinun täytyy `osoittaa ylöspäin`{:class="block3motion"} ja `siirtyä alkuasentoon`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Tässä on tarvitsemasi koodilohkot:

![vene-hahmo](images/boat_resize.png)

```blocks3
jos <touching color [ ] ?> , niin
end

mene sijaintiin x: (-190) y: (-150)

vaihda asusteeksi (osuma v)

osoita suuntaan (0)

vaihda asusteeksi (normaali v)

sano [Eiiiiii!] (2) sekunnin ajan
```

\--- /hint \--- \--- hint \---

Koodisi tulisi näyttää seuraavalta:

![vene-hahmo](images/boat_resize.png)

```blocks3
kun klikataan ⚑
osoita suuntaan (0)
mene sijaintiin x: (-190) y: (-150)
ikuisesti 
  jos <(etäisyys kohteeseen (hiiren osoitin v)) > [5]>, niin 
    osoita kohti (hiiren osoitin v)
    liiku (1) askelta
  end
  jos <touching color [#663b00] ?>, niin 
    vaihda asusteeksi (osuma v)
    sano [Eiiiiii!] (2) sekunnin ajan
    vaihda asusteeksi (normaali v)
    osoita suuntaan (0)
    mene sijaintiin x: (-190) y: (-150)
  end
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Sinun pitäisi myös lisätä koodi varmistaaksesi, että vene aloittaa aina 'normaalissa' asusteessa.

Testaa koodi uudelleen. Jos yrität veneellä purjehtia puisen esteen läpi, veneen tulee törmätä ja sitten siirtyä takaisin alkuasentoonsa.

![kuvakaappaus](images/boat-crash.png)

\--- /task \---