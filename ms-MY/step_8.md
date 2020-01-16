## Halangan dan penggalak

Sekarang permainan ini adalah **jauh** terlalu mudah, supaya anda akan menambah beberapa perkara untuk membuat ia lebih menarik.

Pertama, anda akan menambah beberapa penyokong untuk mempercepatkan bot.

\--- tugas \---

Edit latar belakang Tahap anda dengan menambah beberapa anak panah penggalak putih.

![tangkapan skrin](images/boat-boost.png)

\--- / tugas \---

\--- tugas \---

Sekarang tambahkan lebih banyak blok kod ke perahu anda `selama-lamanya`{: class = "block3control"} gelung supaya sprite kapal bergerak tiga langkah tambahan apabila menyentuh anak panah putih.

![boat-sprite](images/boat_resize.png)

```blocks3
jika <touching color [#FFFFFF] ?> maka
langkah (3) langkah
hujung
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
tamat

putar cw (1) darjah

apabila bendera diklik
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
apabila bendera mengklik
selamanya
putar cw (1) darjah
hujung
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---