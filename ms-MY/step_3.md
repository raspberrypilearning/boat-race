## Mengawal perahu

Pemain akan mengawal sprit bot dengan tetikus.

\--- tugas \--- Tambah kod ke sprite kapal supaya ia bermula di sudut kiri bawah menunjuk ke atas dan kemudian mengikuti penunjuk tetikus.

![bot-sprite](images/boat_resize.png)

```blocks3
apabila bendera diklik
titik ke arah (0)
pergi ke x: (-190) y: (-150)
selamanya
titik ke arah (tetikus-penunjuk v)
langkah (1) langkah
```

\--- / tugas \---

\--- tugas \---

**Uji kod anda** dengan mengklik bendera hijau dan gerakkan tetikus. Adakah kapal sprit bergerak ke arah penunjuk tetikus?

![tangkapan skrin](images/boat-mouse.png)

\--- tidak mencetak \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- / tidak mencetak \---

\--- print-only \--- ![screenshot](images/boat-pointer-test-anim.png) \--- / print-only \---

\--- / tugas \---

\--- tugas \---

Apa yang berlaku apabila bot mencapai penunjuk tetikus? Cuba untuk melihat apa masalahnya.

\--- / tugas \---

\--- tugas \---

Untuk menghentikan ini daripada berlaku, anda perlu menambah `jika`{: class = "block3control"} blok ke kod anda, supaya sprite kapal hanya bergerak jika lebih dari 5 piksel jauh dari penunjuk tetikus.

\--- petunjuk \--- \--- petunjuk \--- Bot hanya perlu menunjuk ke arah penunjuk tetikus dan bergerak `jika`{: class = "block3control"} jarak `ke penunjuk tetikus`{: class = "block3sensing"} adalah `lebih besar daripada 5 piksel`{: class = "block3operators"}. \--- / petunjuk \--- \--- petunjuk \--- Ini adalah blok kode yang anda perlukan untuk menambah kode untuk sprite kapal: ![bot-sprite](images/boat_resize.png)

```blocks3
jika < [] > [] > maka

(jarak ke (mouse-pointer v))
```

\--- / petunjuk \--- \--- petunjuk \--- Ini adalah apa yang kod anda harus kelihatan seperti: ![bot-sprite](images/boat_resize.png)

```blocks3
apabila bendera mengklik
poin ke arah (0)
pergi ke x: (-190) y: (-150)
selamanya
jika <(jarak ke (mouse-pointer v)) > [5]> lalu
titik ke arah (tetikus- penunjuk v)
langkah (1) langkah
```

\--- / petunjuk \--- \--- / petunjuk \---

\--- / tugas \---

\--- tugas \---

Uji kod anda sekali lagi untuk memeriksa sama ada masalah itu telah ditetapkan sekarang.

\--- / tugas \---