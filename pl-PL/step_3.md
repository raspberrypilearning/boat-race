## Sterowanie łodzią

\--- task \---

Add this code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![duszek łodzi](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
point towards (mouse-pointer v)
move (1) steps
```

\--- /task \---

\--- task \---

**Przetestuj swój kod**, klikając zieloną flagę i poruszając myszą. Czy duszek łodzi przesuwa się w kierunku wskaźnika myszy?

![zrzut ekranu](images/boat-mouse.png)

\--- no-print \---

![zrzut ekranu](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![zrzut ekranu](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

Co się stanie, gdy łódź dopłynie do wskaźnika myszy? Wypróbuj, aby zobaczyć, na czym polega problem.

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

Przetestuj swój kod ponownie, aby sprawdzić, czy problem został już rozwiązany.

\--- /task \---