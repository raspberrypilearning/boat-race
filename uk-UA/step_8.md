## Перешкоди і прискорювачі

Зараз гра **на** занадто легко, так що ви додасте деякі речі, щоб зробити її більш цікавою.

По-перше, ви додасте деякі прискорювачі, щоб прискорити човен.

\--- task \---

Відредагуйте фон Stage, додавши до нього деякі білі стрілки.

![скріншот](images/boat-boost.png)

\--- /task \---

\--- task \---

Тепер додайте більше блоків коду до петлі `назавжди`: ![човен-спрайт](images/boat_resize.png)

```blocks3
якщо <touching color [#FFFFFF] ?> потім
переміщення (3) кроків
закінчення
```

\--- /task \---

\--- task \---

Перевірте свою гру, щоб дізнатися, чи прискорять ваш новий прискорювач човна.

\--- /task \---

Далі ви додасте обертальний воріт, якого човен повинен уникати.

\--- task \---

Додайте новий спрайт, який виглядає так, і назвіть його "gate":

![скріншот](images/boat-gate.png)

Переконайтеся, що колір спрайта воріт такий же, як і колір дерев'яних бар'єрів.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![ворота](images/gate.png)

```blocks3
назавжди
кінець

повернути cw (1) градусів

коли прапорець натиснув
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

```blocks3
коли прапор натиснув
назавжди
поворот cw (1) градусів
кінець
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---