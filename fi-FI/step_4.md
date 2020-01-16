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

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

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

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

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

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---