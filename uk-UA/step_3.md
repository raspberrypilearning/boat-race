## Керування човном

Гравець керуватиме спрайтом човна за допомогою миші.

\--- task \---

Додай код до спрайту човна, щоб він розпочинав в лівому нижньому куті і був направлений вгору, а потім слідував за вказівником мишки.

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

Щоб такого не відбувалося, тобі треба додати в свій код блок `якщо`{:class="block3control"}, щоб спрайт човна рухався, тільки коли він знаходиться далі ніж за 5 пікселів від вказівника мишки.

\--- hints \--- \--- hint \---

Човен має бути направлений на вказівник мишки і рухатися, `якщо`{:class="block3control"} `відстань до вказівника мишки`{:class="block3sensing"} `більша за 5 пікселів`{:class="block3operators"}.

\--- /hint \--- \--- hint \---

Ось блоки коду, які тобі треба додати до спрайту човна:

![спрайт човна](images/boat_resize.png)

```blocks3
if < [ ] > [ ] > then

(distance to (mouse-pointer v))
```

\--- /hint \--- \--- hint \---

Ось як має виглядати твій код:

![спрайт човна](images/boat_resize.png)

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

Протестуй свій код знову і перевір, чи проблема зникла.

\--- /task \---