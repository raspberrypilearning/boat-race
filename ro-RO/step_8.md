## Obstacole și propulsatoare

Până acum, jocul este **prea** ușor, așa că vei adăuga unele lucruri pentru a-l face mai interesant.

Prima data, vei adăuga câteva propulsatoare pentru a mări viteza bărcii.

\--- task \---

Editează decorul Scenei tale adăugând câteva săgeți albe propulsatoare.

![captură de ecran](images/boat-boost.png)

\--- /task \---

\--- task \---

Acum, adaugă mai multe blocuri de cod la bucla `la infinit`{:class="block3control"} a bărcii tale pentru ca barca să meargă încă 3 pași când atinge o săgeată albă. ![barcă](images/boat_resize.png)

```blocks3
dacă <atinge culoarea [#FFFFFF]?>
mergi (3) pași
end
```

\--- /task \---

\--- task \---

Testează-ți jocul pentru a vedea dacă noile tale săgeți propulsatoare accelerează barca.

\--- /task \---

În continuare, vei adăuga o poartă rotitoare pe care barca trebuie să o evite.

\--- task \---

Adaugă un personaj nou care arată astfel și denumește-l „poartă”:

![captură de ecran](images/boat-gate.png)

Asigură-te că culoarea porții este aceeași culoare cu culoarea barierelor din lemn.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![poartă](images/gate.png)

```blocks3
la infinit
end

rotește-te la dreapta (1) grade

când se dă click pe stegulețul verde
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

```blocks3
când se dă click pe stegulețul verde
la infinit
rotește-te la dreapta (1) grade
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---