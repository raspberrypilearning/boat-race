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

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
tukar [masa v] dengan (0.1)

apabila bendera diklik

selamanya
tamat

tunggu (0.1) saat

set [masa v] hingga [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
apabila bendera mengklik
set [masa v] ke [0]
selama
menunggu (0.1) saat
perubahan [masa v] oleh (0.1)
akhir
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---