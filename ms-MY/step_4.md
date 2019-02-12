## Crashing!

Pada masa ini, sprit bot hanya dapat berlayar melalui halangan kayu! Anda akan memperbaikinya sekarang.

\--- tugas \---

Anda memerlukan dua kostum untuk sprit bot anda: kostum biasa, dan satu untuk ketika bot terjatuh. Dandakan kostum permaidani bot anda, dan namakan satu kostum 'biasa' dan yang lain 'memukul'.

\--- / tugas \---

\--- tugas \---

Klik pada kostum 'hit' anda, dan gunakan alat **Pilih** untuk merebut keping kostum dan gerakkan dan memutarkannya untuk membuat bot kelihatan seperti ia telah terputus.

![tangkapan skrin](images/boat-hit-costume-annotated.png)

\--- / tugas \---

\--- tugas \---

Sekarang tambahkan kod ke bot anda supaya ia terhempas dan pecah apabila ia menyentuh sebarang halangan kayu coklat.

\--- petunjuk \--- \--- petunjuk \--- Anda perlu menambah blok kod di dalam gelung `{`=} block3control "} untuk selama-lamanya supaya kod anda terus memeriksa jika sprit kapal telah terhempas, dan jika ia telah terhempas, kod tersebut perlu menetapkan semula kedudukan sprit bot.

`jika`{: class = "block3control"} perahu adalah `menyentuh`{: class = "block3sensing"} warna coklat kayu, anda perlu `beralih ke pakaian hit`{: class = "block3looks"} , `katakan Noooo! untuk 2 saat`{: class = "block3looks"}, dan kemudian `bertukar kepada pakaian biasa`{: class = "block3looks"}. Akhirnya, anda perlu `titik`{: class = "block3motion"} dan `pergi ke kedudukan mula`{: class = "block3motion"}.

\--- / petunjuk \--- \--- petunjuk \--- Berikut adalah blok kode yang anda perlukan: ![bot-sprite](images/boat_resize.png)

```blocks3
jika <touching color [ ] ?> maka
hujung

pergi ke x: (-190) y: (-150)

suis pakaian ke (hit v)

mata ke arah (0)

suis suis ke (v normal)

katakan [Noooooo!] (2) saat
```

\--- / petunjuk \--- \--- petunjuk \--- Inilah kodanya yang seharusnya seperti: ![bot-sprite](images/boat_resize.png)

```blocks3
apabila bendera mengklik
poin ke arah (0)
pergi ke x: (-190) y: (-150)
selamanya
jika <(jarak ke (mouse-pointer v)) > [5]> lalu
titik ke arah (tetikus- penunjuk v)
langkah (1) tidak perlu pergi
akhir
jika <touching color [#663b00] ?> kemudian
suis pakaian untuk (hit v)
mengatakan [noooooo!] untuk (2) saat
suis pakaian untuk (v normal)
titik dalam arah (0)
pergi ke x: (-190) y: (-150)
akhir
```

\--- / petunjuk \--- \--- / petunjuk \---

\--- / tugas \---

\--- tugas \---

Anda juga perlu menambah kod untuk memastikan bahawa bot sprit anda sentiasa bermula mencari 'normal'.

Uji kod anda sekali lagi. Sekiranya anda cuba melayari bot itu melalui penghalang kayu sekarang, bot itu akan terhempas dan kemudian kembali ke kedudukan permulaannya.

![tangkapan skrin](images/boat-crash.png)

\--- / tugas \---