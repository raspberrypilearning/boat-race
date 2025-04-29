## De boot besturen

\--- task \---

Add this code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![boot-sprite](images/boat_resize.png)

```blocks3
wanneer op groene vlag wordt geklikt
richt naar (0) graden
ga naar x: (-190) y: (-150)
herhaal
richt naar (muisaanwijzer v)
neem (1) stappen
```

\--- /task \---

\--- task \---

**Test je code ** door op de groene vlag te klikken en de muis te verplaatsen. Beweegt de boot-sprite in de richting van de muisaanwijzer?

![screenshot](images/boat-mouse.png)

\--- no-print \---

![screenshot](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![screenshot](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

Wat gebeurt er als de boot de muisaanwijzer bereikt? Probeer het uit om te zien wat het probleem is.

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

Test je code opnieuw om te controleren of het probleem is opgelost.

\--- /task \---