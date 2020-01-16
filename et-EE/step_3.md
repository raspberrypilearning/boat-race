## Paadi juhtimine

Mängija kontrollib paadi sprite hiirega.

\--- task \---

Add code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![boat-sprite](images/boat_resize.png)

```blocks3
kui lipp klõpsas
punkti suunas (0)
minge x: (-190) y: (-150)
igavesti
punkti (hiirekursor v)
liiguta (1) sammu suunas
```

\--- /task \---

\--- task \---

**Test your code** by clicking the green flag and moving the mouse. Does the boat sprite move towards the mouse pointer?

![screenshot](images/boat-mouse.png)

\--- no-print \---

![screenshot](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![screenshot](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

What happens when the boat reaches the mouse pointer? Try it out to see what the problem is.

\--- /task \---

\--- task \---

To stop this from happening, you need to add an `if`{:class="block3control"} block to your code, so that the boat sprite only moves if it is more than 5 pixels away from the mouse pointer.

\--- hints \--- \--- hint \---

The boat should only point towards the mouse pointer and move `if`{:class="block3control"} the `distance to the mouse pointer`{:class="block3sensing"} is `greater than 5 pixels`{:class="block3operators"}.

\--- /hint \--- \--- hint \---

These are the code blocks you need to add to the code for the boat sprite:

![boat-sprite](images/boat_resize.png)

```blocks3
kui < [] > [] > siis

(kaugus (hiirekursor v))
```

\--- /hint \--- \--- hint \---

This is what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
kui lipp klõpsas
punkti suunas (0)
minge x: (-190) y: (-150)
igavesti
kui <(kaugus (hiirekursor v)) > [5]> siis
punkti (hiir- pointer v)
liiguta (1) samme
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your code again to check whether the problem is now fixed.

\--- /task \---