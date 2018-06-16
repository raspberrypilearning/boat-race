## Upravljanje brodom

\--- task \---

Brodom ćeš upravljati pomoću miša. Dodaj naredbe svom brodu tako da krene iz donjeg lijevog kuta okrenut prema gore i slijedi pokazivač miša. **Testiraj svoj kod** kako bi se uvjerio da radi ono što bi trebao.

\--- hints \--- \--- hint \--- Kad je `kliknuta zelena zastavica`, tvoj brod treba `otići na početnu poziciju` i `okrenuti se prema gore`. Next it will need to `point towards the mouse pointer` and `move 1 step`. It will need to repeat this `forever`.

\--- /hint \--- \--- hint \--- Here are the code blocks you'll need: ![screenshot](images/boat-move-blocks.png) \--- /hint \--- \--- hint \--- This is what your code should look like: ![screenshot](images/boat-move-code.png) \--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your boat by clicking the flag and moving the mouse. Does the boat sail towards the mouse?

![screenshot](images/boat-mouse.png)

![screenshot](images/boat-pointer-test-anim.gif)

## \--- collapse \---

title: If you have problems ...

## image: images/image.png

**Note:** There is currently a bug in Scratch which means your boat may not move towards the mouse pointer. If this happens, click the arrow on the `point towards` block and re-select `mouse-pointer`.

![screenshot](images/boat-bug.png) \--- /collapse \---

\--- /task \---

\--- task \---

What happens if the boat reaches the mouse pointer? Try it.

\--- /task \---

\--- task \---

To stop this from happening, you'll need to add an `if` block to your code, so that the boat only moves if it is more than 5 pixels away from the mouse.

\--- hints \--- \--- hint \--- The boat should only point towards the mouse pointer and move `if` the `distance to the mouse pointer` is `greater than 5 pixels`. \--- /hint \--- \--- hint \--- Here are the code blocks you'll need to add to the code for the boat: ![screenshot](images/boat-pointer-blocks.png) \--- /hint \--- \--- hint \--- This is what your code should look like: ![screenshot](images/boat-pointer-code.png) \--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your boat again to check whether the problem has been fixed.

\--- /task \---