## Kemenangan!

\--- task \--- Sekarang tambahkan pernyataan `if`{: class = "block3control"} ke kode sprite kapal Anda sehingga pemain menang ketika mereka membuat kapal tiba di pulau kuning.

Ketika kapal sampai ke pulau itu, permainan harus mengatakan 'YEAH!', Dan kemudian harus berakhir.

\--- hints \--- \--- hint \--- Anda perlu menambahkan lebih banyak blok kode di dalam `selamanya`{: class = "block3control"} agar kode Anda terus memeriksa apakah pemain telah menang:

`jika`{: class = "block3control"} perahu `menyentuh`{: class = "block3sensing"} warna pulau, Anda perlu `mengatakan 'YEAH! selama 2 detik`{: class = "block3looks"} dan kemudian `hentikan semua`{: class = "block3control"} untuk mengakhiri permainan. \--- / hint \--- \--- hint \--- Ini adalah blok kode yang Anda butuhkan: ![perahu-sprite](images/boat_resize.png)

```blocks3
katakan [YEAH!] untuk (2) detik

jika <touching color [#FFFF99] ?> lalu


berhenti [semua v]

```

\--- / hint \--- \--- hint \--- Begini tampilannya kode baru Anda: ![perahu-sprite](images/boat_resize.png)

```blocks3
jika <touching color [#FFFF99] ?> maka
katakan [YEAH!] selama (2) detik
hentikan [all v]
end
```

Jangan lupa bahwa kode baru ini harus berada di dalam loop `selamanya`{: class = "block3control"}. \--- / petunjuk \--- \--- / petunjuk \--- \--- / tugas \---