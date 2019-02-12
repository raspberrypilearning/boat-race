## Menambah pemasa

Sekarang anda akan menambah pemasa untuk permainan anda, supaya pemain perlu sampai ke pulau secepat mungkin.

\--- tugas \---

Tambah pembolehubah baru yang dipanggil `masa`{: class = "block3variables"} ke Peringkat anda.

![tangkapan skrin](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Anda juga boleh memilih mencari pemasa anda dengan mengubah cara pembolehubah baru anda dipaparkan.

\--- / tugas \---

\--- tugas \---

Sekarang tambahkan blok kod ke Tahap anda supaya pemasa mengira sehingga bot sampai ke pulau itu.

\--- petunjuk \--- \--- petunjuk \--- Pada Tahap, `apabila bendera hijau diklik`{: class = "block3control"}, `tetapkan masa untuk 0`{: class = "block3variables "}. Di dalam anda `selama-lamanya`{: class = "block3control"} gelung, anda akan perlu terlebih dahulu `tunggu 0,1 secs`{: class = "block3control"}, kemudian `perubahan masa 0.1`{: class = "block3variables" }. \--- / petunjuk \--- \--- petunjuk \--- Berikut adalah blok kode yang anda perlukan: ![pentas](images/stage.png)

```blocks3
tukar [masa v] dengan (0.1)

apabila bendera diklik

selamanya
tamat

tunggu (0.1) saat

set [masa v] hingga [0]
```

\--- / petunjuk \--- \--- petunjuk \--- Berikut adalah kod baru anda yang seharusnya kelihatan seperti: ![pentas](images/stage.png)

```blocks3
apabila bendera mengklik
set [masa v] ke [0]
selama
menunggu (0.1) saat
perubahan [masa v] oleh (0.1)
akhir
```

\--- / petunjuk \--- \--- / petunjuk \---

\--- / tugas \---

\--- tugas \---

Uji permainan anda dan lihat betapa cepat anda boleh mendapatkan bot ke pulau itu!

![tangkapan skrin](images/boat-variable-test.png)

\--- / tugas \---