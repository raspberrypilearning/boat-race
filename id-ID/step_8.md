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

\--- /tugas \---

\--- tugas \---

Pastikan bahwa tengah sprite gerbang diposisikan di tengah.

![tangkapan layar](images/boat-center.png)

\--- /tugas \---

\--- tugas \---

Tambahkan kode ke sprite gerbang Anda untuk membuatnya berputar perlahan selamanya.

\--- hints \--- \--- hint \--- Tambahkan blok kode ke gerbang sprite sehingga `ternyata 1 derajat`{: class = "block3motion"} `selamanya`{: class = "block3control"} . \--- / hint \--- \--- hint \--- Ini adalah blok kode yang Anda butuhkan: ![gerbang](images/gate.png)

```blocks3
selamanya
end

turn cw (1) derajat

saat flag diklik
```

\--- / hint \--- \--- hint \--- Begini tampilannya kode baru Anda: ![gerbang](images/gate.png)

```blocks3
ketika flag diklik
selamanya
turn cw (1) derajat
end
```

\--- / hint \--- \--- / hints \---

\--- /tugas \---

\--- tugas \---

Uji lagi permainan Anda. Anda sekarang harus memiliki gerbang pemintalan yang Anda butuhkan untuk menggerakkan perahu Anda.

![tangkapan layar](images/boat-gate-test.png)

\--- /tugas \---