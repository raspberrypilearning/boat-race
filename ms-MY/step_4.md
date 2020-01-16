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

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
jika <touching color [ ] ?> maka
hujung

pergi ke x: (-190) y: (-150)

suis pakaian ke (hit v)

mata ke arah (0)

suis suis ke (v normal)

katakan [Noooooo!] (2) saat
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

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

\--- /hint \--- \--- /hints \---

\--- / tugas \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---