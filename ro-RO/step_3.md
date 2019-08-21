## Controlarea barcii

Jucătorul va controla barca cu mouse-ul.

\--- task \--- Adaugă codul pentru ca barca să fie poziționată în colțul din stânga jos, cu fața în sus, iar apoi să urmărească poziția cursorului.

![barcă](images/boat_resize.png)

```blocks3
când se dă click pe stegulețul verde
orientează-te în direcția (0)
mergi la x: (-190) y: (-150)
la infinit
orientează-te spre (cursorul mouse-ului v)
mergi (1) pași
```

\--- /task \---

\--- task \---

**Testează-ți codul** dând click pe steagul verde și mișcându-ți mouse-ul. Barca se mișcă spre săgeata mouse-ului?

![captură de ecran](images/boat-mouse.png)

\--- no-print \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- /no-print \---

\--- print-only \--- ![screenshot](images/boat-pointer-test-anim.png) \--- /print-only \---

\--- /task \---

\--- task \---

Ce se intâmplă când barca ajunge la săgeata mouse-ului? Încearcă și vezi care e problema.

\--- /task \---

\--- task \---

Pentru a preveni acest lucru, trebuie să adaugi un bloc `dacă`{:class="block3control"} la codul tău, astfel încât barca să se miște dacă este la o distanță de 5 pixeli de săgeata mouse-ului.

\--- hints \--- \--- hint \--- Barca ar trebui să fie îndreptată doar spre săgeata mouse-ului și să se miște doar `dacă`{:class="block3control"} `distanța până la cursorul mouse-ului`{:class="block3sensing"} este `> 5 pixeli`{:class="block3operators"}. \--- /hint \--- \--- hint \--- Acestea sunt blocurile de cod pe care trebuie să le adaugi la codul pentru barcă: ![barcă](images/boat_resize.png)

```blocks3
dacă < [ ] > [ ] > atunci

(distanța până la (cursorul mouse-ului v))
```

\--- /hint \--- \--- hint \--- Așa ar trebui să arate codul: ![barcă](images/boat_resize.png)

```blocks3
când se dă click pe stegulețul verde
orientează-te în direcția (0)
mergi la x: (-190) y: (-150)
la infinit
dacă <(distanța până la (cursorul mouse-ului v)) > [5]> atunci
orientează-te spre (cursorul mouse-ului v)
mergi (1) pași
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Testează-ți codul din nou pentru a vedea dacă problema a dispărut.

\--- /task \---