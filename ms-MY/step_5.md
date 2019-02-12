## Memenangi!

\--- tugas \--- Sekarang masukkan lagi `jika`{: class = "block3control"} kepada kod sprite anda supaya pemain menang ketika mereka membuat bot tiba di pulau kuning.

Apabila bot itu sampai ke pulau itu, permainan itu harus mengatakan 'YEAH!', Dan kemudian ia harus berakhir.

\--- petunjuk \--- \--- petunjuk \--- Anda perlu menambah lebih blok kod dalam anda `selama-lamanya`{: class = "block3control"} gelung supaya kod anda menyimpan memeriksa jika pemain telah dimenangi:

`jika`{: class = "block3control"} bot adalah `menyentuh`{: class = "block3sensing"} warna pulau, anda perlu `katakan 'YEAH!' selama 2 saat`{: class = "block3looks"} dan kemudian `stop semua`{: class = "block3control"} untuk menamatkan permainan. \--- / petunjuk \--- \--- petunjuk \--- Berikut adalah blok kode yang anda perlukan: ![bot-sprite](images/boat_resize.png)

```blocks3
katakan [YEAH!] untuk (2) saat

jika <touching color [#FFFF99] ?> maka
hujung

berhenti [semua v]

```

\--- / petunjuk \--- \--- petunjuk \--- Berikut adalah kod baru anda yang seharusnya kelihatan seperti: ![bot-sprite](images/boat_resize.png)

```blocks3
jika <touching color [#FFFF99] ?> maka
berkata [YEAH!] untuk (2) saat
berhenti [semua v]
akhir
```

Jangan lupa bahawa kod baru ini perlu berada di dalam `selama`{: class = "block3control"} gelung. \--- / petunjuk \--- \--- / petunjuk \--- \--- / tugas \---