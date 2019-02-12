## Mengontrol perahu

Pemain akan mengendalikan sprite kapal dengan mouse.

\--- task \--- Tambahkan kode ke sprite perahu sehingga dimulai di sudut kiri bawah mengarah ke atas dan kemudian mengikuti pointer mouse.

![perahu-sprite](images/boat_resize.png)

```blocks3
ketika bendera diklik
titik searah (0)
pergi ke x: (-190) y: (-150)
selamanya
titik ke arah (penunjuk mouse v)
langkah (1) langkah
```

\--- /tugas \---

\--- tugas \---

**Uji kode Anda** dengan mengeklik bendera hijau dan menggerakkan mouse. Apakah sprite perahu bergerak ke arah penunjuk mouse?

![tangkapan layar](images/boat-mouse.png)

\--- tanpa cetak \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- / tanpa cetak \---

\--- hanya cetak \--- ![screenshot](images/boat-pointer-test-anim.png) \--- / hanya cetak \---

\--- /tugas \---

\--- tugas \---

Apa yang terjadi ketika kapal mencapai pointer mouse? Cobalah untuk melihat apa masalahnya.

\--- /tugas \---

\--- tugas \---

Agar hal ini tidak terjadi, Anda perlu menambahkan blok `jika`{: class = "block3control"} ke kode Anda, sehingga sprite kapal hanya bergerak jika jaraknya lebih dari 5 piksel dari penunjuk mouse.

\--- hints \--- \--- hint \--- Perahu seharusnya hanya mengarah ke pointer mouse dan bergerak `jika`{: class = "block3control"} `jarak ke pointer mouse`{: class = "block3sensing"} adalah `lebih besar dari 5 piksel`{: class = "block3operators"}. \--- / hint \--- \--- hint \--- Ini adalah blok kode yang perlu Anda tambahkan ke kode untuk sprite kapal: ![perahu-sprite](images/boat_resize.png)

```blocks3
jika < [] > [] > maka

(jarak ke (penunjuk mouse v))
```

\--- / hint \--- \--- hint \--- Beginilah tampilan kode Anda: ![perahu-sprite](images/boat_resize.png)

```blocks3
ketika bendera diklik
titik ke arah (0)
pergi ke x: (-190) y: (-150)
selamanya
jika <(jarak ke (mouse-pointer v)) > [5]> lalu
titik ke arah (mouse- pointer v)
langkah (1) langkah
```

\--- / hint \--- \--- / hints \---

\--- /tugas \---

\--- tugas \---

Uji kembali kode Anda untuk memeriksa apakah masalahnya sudah diperbaiki.

\--- /tugas \---