## Menabrak!

Pada saat ini, sprite kapal dapat dengan mudah melewati penghalang kayu! Anda akan memperbaikinya sekarang.

\--- tugas \---

Anda membutuhkan dua kostum untuk sprite kapal Anda: satu kostum normal, dan satu lagi untuk saat kapal menabrak. Gandakan kostum sprite kapal Anda, dan beri nama satu kostum 'normal' dan yang lainnya 'hit'.

\--- /tugas \---

\--- tugas \---

Klik pada kostum 'hit' Anda, dan gunakan alat **Select** untuk mengambil bagian-bagian dari kostum dan bergerak dan putar untuk membuat perahu terlihat seperti telah hancur berkeping-keping.

![tangkapan layar](images/boat-hit-costume-annotated.png)

\--- /tugas \---

\--- tugas \---

Sekarang tambahkan kode ke kapal Anda sehingga crash dan pecah ketika menyentuh setiap rintangan kayu berwarna coklat.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
jika <touching color [ ] ?> maka
akhir

pergi ke x: (-190) y: (-150)

beralih kostum ke (tekan v)

titik arah (0)

beralih kostum ke (normal v)

katakan [Tidaaaaaak!] untuk (2 detik
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
ketika bendera diklik
titik ke arah (0)
pergi ke x: (-190) y: (-150)
selamanya
jika <(jarak ke (mouse-pointer v)) > [5]> lalu
titik ke arah (mouse- pointer v)
pindah (1) langkah
end
jika <touching color [#663b00] ?> kemudian
beralih kostum ke (tekan v)
katakan [Tidaaaaaak!] untuk (2) detik
beralih kostum ke (normal v)
titik arah (0)
pergi ke x: (-190) y: (-150)
akhir
```

\--- /hint \--- \--- /hints \---

\--- /tugas \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---