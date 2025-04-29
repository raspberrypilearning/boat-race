## Veneen ohjaaminen

\--- task \---

Add this code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![vene-hahmo](images/boat_resize.png)

```blocks3
kun klikataan ⚑
osoita suuntaan (0)
mene sijaintiin x: (-190) y: (-150)
ikuisesti 
  osoita kohti (mouse-pointer v)
  liiku (1) askelta
end
```

\--- /task \---

\--- task \---

**Testaa koodi** klikkaamalla vihreää lippua ja liikuttamalla hiirtä. Liikkuuko vene kohti hiiren osoitinta?

![kuvakaappaus](images/boat-mouse.png)

\--- no-print \---

![kuvakaappaus](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![kuvakaappaus](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

Mitä tapahtuu, kun vene saavuttaa hiiren osoittimen? Kokeile sitä, jotta näet mikä ongelma on.

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

Testaa koodi uudelleen tarkistaaksesi, onko ongelma nyt korjattu.

\--- /task \---