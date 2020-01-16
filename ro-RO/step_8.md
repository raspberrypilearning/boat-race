## Obstacole și propulsatoare

Până acum, jocul este **prea** ușor, așa că vei adăuga unele lucruri pentru a-l face mai interesant.

Prima data, vei adăuga câteva propulsatoare pentru a mări viteza bărcii.

\--- task \---

Editează decorul Scenei tale adăugând câteva săgeți albe propulsatoare.

![captură de ecran](images/boat-boost.png)

\--- /task \---

\--- task \---

Acum, adaugă mai multe blocuri de cod la bucla `la infinit`{:class="block3control"} a bărcii tale pentru ca barca să meargă încă 3 pași când atinge o săgeată albă.

![boat-sprite](images/boat_resize.png)

```blocks3
dacă <atinge culoarea [#FFFFFF]?>
mergi (3) pași
end
```

\--- /task \---

\--- task \---

Test your game to see whether your new booster arrows speed up the boat.

\--- /task \---

Next you'll add a spinning gate that the boat has to avoid.

\--- task \---

Add a new sprite that looks like this, and call it 'gate':

![screenshot](images/boat-gate.png)

Make sure that the colour of the gate sprite is the same as the colour of the wooden barriers.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \---

Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![gate](images/gate.png)

```blocks3
la infinit
end

rotește-te la dreapta (1) grade

când se dă click pe stegulețul verde
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

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