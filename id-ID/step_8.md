## Hambatan dan pemacu

Saat ini gim ini **jauh** terlalu mudah, jadi Anda akan menambahkan beberapa hal untuk membuatnya lebih menarik.

Pertama, Anda akan menambahkan beberapa booster untuk mempercepat kapal.

\--- tugas \---

Edit latar panggung Anda dengan menambahkan beberapa panah penguat putih.

![tangkapan layar](images/boat-boost.png)

\--- /tugas \---

\--- tugas \---

Sekarang tambahkan lebih banyak blok kode ke loop `selamanya`kapal Anda {: class = "block3control"} sehingga sprite perahu memindahkan tiga langkah tambahan saat menyentuh panah putih. ![perahu-sprite](images/boat_resize.png)

```blocks3
jika <touching color [#FFFFFF] ?> maka
langkah (3) langkah
berakhir
```

\--- /tugas \---

\--- tugas \---

Uji permainan Anda untuk melihat apakah panah pendorong baru Anda mempercepat kapal.

\--- /tugas \---

Selanjutnya Anda akan menambahkan gerbang pemintalan yang harus dihindari kapal.

\--- tugas \---

Tambahkan sprite baru yang terlihat seperti ini, dan menyebutnya 'gerbang':

![tangkapan layar](images/boat-gate.png)

Pastikan warna gerbang sprite sama dengan warna penghalang kayu.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![gerbang](images/gate.png)

```blocks3
selamanya
end

turn cw (1) derajat

saat flag diklik
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

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