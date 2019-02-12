## Halangan dan penggalak

Sekarang permainan ini adalah **jauh** terlalu mudah, supaya anda akan menambah beberapa perkara untuk membuat ia lebih menarik.

Pertama, anda akan menambah beberapa penyokong untuk mempercepatkan bot.

\--- tugas \---

Edit latar belakang Tahap anda dengan menambah beberapa anak panah penggalak putih.

![tangkapan skrin](images/boat-boost.png)

\--- / tugas \---

\--- tugas \---

Sekarang tambahkan lebih banyak blok kod ke perahu anda `selama-lamanya`{: class = "block3control"} gelung supaya sprite kapal bergerak tiga langkah tambahan apabila menyentuh anak panah putih. ![bot-sprite](images/boat_resize.png)

```blocks3
jika <touching color [#FFFFFF] ?> maka
langkah (3) langkah
hujung
```

\--- / tugas \---

\--- tugas \---

Uji permainan anda untuk melihat sama ada anak panah penggalak baru anda mempercepatkan bot.

\--- / tugas \---

Seterusnya anda akan menambah gerbang berputar yang perlu dielakkan oleh bot.

\--- tugas \---

Tambah sprit baru yang kelihatan seperti ini, dan panggil ia 'pintu':

![tangkapan skrin](images/boat-gate.png)

Pastikan warna sprit pintu adalah sama dengan warna halangan kayu.

\--- / tugas \---

\--- tugas \---

Pastikan pusat sprit pintu ditempatkan di tengah.

![tangkapan skrin](images/boat-center.png)

\--- / tugas \---

\--- tugas \---

Tambah kod ke sprite pintu anda untuk membuat ia berputar perlahan-lahan selama-lamanya.

\--- petunjuk \--- \--- petunjuk \--- Tambah blok kod untuk bidadari pintu supaya ia `bertukar 1 darjah`{: class = "block3motion"} `selama-lamanya`{: class = "block3control"} . \--- / petunjuk \--- \--- petunjuk \--- Berikut adalah blok kode yang anda perlukan: ![pintu gerbang](images/gate.png)

```blocks3
selamanya
tamat

putar cw (1) darjah

apabila bendera diklik
```

\--- / petunjuk \--- \--- petunjuk \--- Berikut adalah kod baru anda yang seharusnya kelihatan seperti: ![pintu gerbang](images/gate.png)

```blocks3
apabila bendera mengklik
selamanya
putar cw (1) darjah
hujung
```

\--- / petunjuk \--- \--- / petunjuk \---

\--- / tugas \---

\--- tugas \---

Uji permainan anda sekali lagi. Anda kini perlu mempunyai pintu berputar yang perlu anda pancarkan bot anda.

![tangkapan skrin](images/boat-gate-test.png)

\--- / tugas \---