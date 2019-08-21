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

\--- /task \---

\--- task \---

Asigură-te că centrul porții este poziționat în mijloc.

![captură de ecran](images/boat-center.png)

\--- /task \---

\--- task \---

Adaugă cod la poarta ta pentru a o face să se rotească ușor la infinit.

\--- hints \--- \--- hint \--- Adaugă blocuri de cod la poartă pentru a o `roti 1 grad`{:class="block3motion"} `la infinit`{:class="block3control"}. \--- /hint \--- \--- hint \--- Iată blocurile de cod de care ai nevoie: ![poartă](images/gate.png)

```blocks3
la infinit
end

rotește-te la dreapta (1) grade

când se dă click pe stegulețul verde
```

\--- /hint \--- \--- hint \--- Așa ar trebui să arate codul: ![poartă](images/gate.png)

```blocks3
când se dă click pe stegulețul verde
la infinit
rotește-te la dreapta (1) grade
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Testează-ți jocul din nou. Ar trebui să ai o poartă rotitoare pe care trebuie să o ferești de barca ta.

![captură de ecran](images/boat-gate-test.png)

\--- /task \---