## Menambahkan penghitung waktu

Sekarang Anda akan menambahkan timer ke gim Anda, sehingga pemain harus pergi ke pulau secepat mungkin.

\--- tugas \---

Tambahkan variabel baru bernama `waktu`{: class = "block3variables"} ke Tahap Anda.

![tangkapan layar](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Anda juga dapat memilih tampilan timer Anda dengan mengubah cara variabel baru Anda ditampilkan.

\--- /tugas \---

\--- tugas \---

Sekarang tambahkan blok kode ke Tahap Anda sehingga penghitung waktu menghitung sampai perahu mencapai pulau.

\--- hints \--- \--- hint \--- Di Panggung, `ketika bendera hijau diklik`{: class = "block3control"}, `set waktu ke 0`{: class = "block3variables "}. Di dalam `selamanya`{: class = "block3control"} Anda, Anda harus terlebih dahulu `menunggu 0,1 detik`{: class = "block3control"}, lalu `ubah waktu menjadi 0,1`{: class = "block3variables" }. \--- / hint \--- \--- hint \--- Ini adalah blok kode yang Anda perlukan: ![tahap](images/stage.png)

```blocks3
ubah [waktu v] dengan (0,1)

saat bendera diklik

selamanya
berakhir

tunggu (0,1) detik

set [waktu v] menjadi [0]
```

\--- / hint \--- \--- hint \--- Begini tampilannya kode baru Anda: ![tahap](images/stage.png)

```blocks3
ketika bendera diklik
atur [waktu v] ke [0]
selamanya
tunggu (0,1) detik
ubah [waktu v] oleh (0,1)
akhir
```

\--- / hint \--- \--- / hints \---

\--- /tugas \---

\--- tugas \---

Uji permainan Anda dan lihat seberapa cepat Anda bisa mendapatkan kapal ke pulau!

![tangkapan layar](images/boat-variable-test.png)

\--- /tugas \---