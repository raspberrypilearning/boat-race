## Hambatan dan pemacu

Saat ini gim ini **jauh** terlalu mudah, jadi Anda akan menambahkan beberapa hal untuk membuatnya lebih menarik.

Pertama, Anda akan menambahkan beberapa booster untuk mempercepat kapal.

\--- tugas \---

Edit latar panggung Anda dengan menambahkan beberapa panah penguat putih.

![tangkapan layar](images/boat-boost.png)

\--- /tugas \---

\--- tugas \---

Sekarang tambahkan lebih banyak blok kode ke loop `selamanya`kapal Anda {: class = "block3control"} sehingga sprite perahu memindahkan tiga langkah tambahan saat menyentuh panah putih.

![boat-sprite](images/boat_resize.png)

```blocks3
jika <touching color [#FFFFFF] ?> maka
langkah (3) langkah
berakhir
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
selamanya
end

turn cw (1) derajat

saat flag diklik
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
ketika flag diklik
selamanya
turn cw (1) derajat
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---