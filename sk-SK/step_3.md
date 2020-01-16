## Ovládanie lode

Hráč bude ovládať loďku myšou.

\--- task \---

Pridaj scenár ku postave loďky tak, aby začínala v ľavom dolnom rohu a smerovala nahor a potom aby nasledovala ukazovateľ myši.

![postava loďky](images/boat_resize.png)

```blocks3
pri kliknutí na ⚑
smerom (0)
skoč na x: (-190) y: (-150)
opakuj stále 
  smerom k (myš v)
  dopredu (1)
end
```

\--- /task \---

\--- task \---

**Vyskúšaj si scenár** kliknutím na zelenú vlajku a pohybom myši. Pohybuje sa loďka smerom ku ukazovateľu myši?

![snímka obrazovky](images/boat-mouse.png)

\--- no-print \---

![snímka obrazovky](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![snímka obrazovky](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

Čo sa stane, keď loďka príde ku ukazovateľu myši? Vyskúšaj si to, aby si zistil/-a kde sa stala chyba.

\--- /task \---

\--- task \---

Aby si opravil/-a chybu, musíš pridať do scenára blok `ak`{:class="block3control"}, tak aby sa loďka pohybovala len, ak bude vzdialená od ukazovateľa myši viac ako 5 pixelov.

\--- hints \--- \--- hint \---

Loďka by mala smerovať k ukazovateľu myši a pohybovať sa len `ak`{:class="block3control"} `vzdialenosť k myši`{:class="block3sensing"} je `väčšia ako 5 pixelov`{:class="block3operators"}.

\--- /hint \--- \--- hint \---

Toto sú bloky, ktoré potrebuješ pridať k postave svojej loďky:

![postava loďky](images/boat_resize.png)

```blocks3
ak <[ ] > [ ]>
end

(vzdialenosť k (myš v))
```

\--- /hint \--- \--- hint \---

Takto by mal vyzerať tvoj scenár:

![postava loďky](images/boat_resize.png)

```blocks3
pri kliknutí na ⚑
smerom (0)
skoč na x: (-190) y: (-150)
opakuj stále 
  ak <(vzdialenosť k (myš v)) > [5]> 
    smerom k (myš v)
    dopredu (1)
  end
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Vyskúšaj si znovu svoj scenár, aby si zistil/-a, či je chyba opravená.

\--- /task \---