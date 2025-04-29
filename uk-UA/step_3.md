## Керування човном

\--- task \---

Add this code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![спрайт човна](images/boat_resize.png)

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

**Протестуй свій код**, натиснувши зелений прапор і переміщуючи мишку. Чи спрайт човна рухається до вказівника мишки?

![знімок екрана](images/boat-mouse.png)

\--- no-print \---

![знімок екрана](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![знімок екрана](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

Що відбувається, коли човен доходить до вказівника? Перевір це, щоб побачити, в чому саме проблема.

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

Протестуй свій код знову і перевір, чи проблема зникла.

\--- /task \---