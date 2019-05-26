## Ovládanie lode

Hráč bude ovládať loď myšou.

\--- task \--- Pridaj kód postave lode tak, aby začínala v ľavom dolnom rohu a smerovala nahor. Potom aby nasledovala ukazovateľ myši.

![postava lodi](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
point towards (myš v)
move (1) steps
```

\--- /task \---

\--- task \---

**Otestuj svoj kód** kliknutím na zelenú vlajku a pohybom myši. Pohybuje sa postava lode smerom k ukazovateľu myši?

![snímka obrazovky](images/boat-mouse.png)

\--- no-print \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- /no-print \---

\--- print-only \--- ![screenshot](images/boat-pointer-test-anim.png) \--- /print-only \---

\--- /task \---

\--- task \---

Čo sa stane, keď loď dosiahne ukazovateľ myši? Vyskúšaj si to, aby si zistil čo je problém.

\--- /task \---

\--- task \---

Aby si to zastavil, musíš pridať blok kódu `ak`{:class="block3control"}, takže loď sa bude pohybovať len ak bude vzdialená od ukazovateľa myši viac ako 5 pixelov.

\--- hints \--- \--- hint \--- Loď by mala smerovať k ukazovateľu myši a pohybovať sa len `ak`{:class="block3control"} `vzdialenosť k myši`{:class="block3sensing"} je `väčšia ako 5 pixelov`{:class="block3operators"}. \--- /hint \--- \--- hint \--- Toto sú bloky kódu, ktoré potrebuješ pridať k postave svojej lodi: ![postava lodi](images/boat_resize.png)

```blocks3
ak <[ ] > [ ]>
end

(vzdialenosť k (myš v))
```

\--- /hint \--- \--- hint \--- Takto by tvoj kód mal vyzerať: ![postava lodi](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Znova otestuj svoj kód, aby si zistil, či je problém odstránený.

\--- /task \---