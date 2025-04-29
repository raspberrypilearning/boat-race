## Upravljanje čolna

\--- task \---

Add this code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![figura čolna](images/boat_resize.png)

```blocks3
ko kliknemo na zastavico
obrni se v smer (0)
pojdi na x: (-190) y: (-150)
ponavljaj
obrni se proti (kazalcu miške v)
pojdi (1) korakov
```

\--- /task \---

\--- task \---

**Preveri svojo kodo** s klikom na zeleno zastavico in premikanjem miške. Ali se figura ladje premakne proti kazalcu miške?

![posnetek zaslona](images/boat-mouse.png)

\--- no-print \---

![posnetek zaslona](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![posnetek zaslona](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

Kaj se zgodi, ko čoln doseže kazalec miške? Preizkusi, da vidiš, v čem je težava.

\--- /task \---

\--- task \---

Add code to the boat sprite so it only point towards the mouse pointer and moves `if`{:class="block3control"} the `distance to the mouse pointer`{:class="block3sensing"} is `greater than 5 pixels`{:class="block3operators"}.

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
+if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

\--- /task \---

\--- task \---

Ponovno preizkusi svojo kodo in preveri ali je težava odpravljena.

\--- /task \---