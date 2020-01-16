## Перешкоди і прискорювачі

Зараз гра **на** занадто легко, так що ви додасте деякі речі, щоб зробити її більш цікавою.

По-перше, ви додасте деякі прискорювачі, щоб прискорити човен.

\--- task \---

Відредагуйте фон Stage, додавши до нього деякі білі стрілки.

![скріншот](images/boat-boost.png)

\--- /task \---

\--- task \---

Тепер додайте більше блоків коду до петлі `назавжди`:

![boat-sprite](images/boat_resize.png)

```blocks3
якщо <touching color [#FFFFFF] ?> потім
переміщення (3) кроків
закінчення
```

\--- /task \---

\--- task \---

Test your game to see whether your new booster arrows speed up the boat.

\--- /task \---

Next you'll add a spinning gate that the boat has to avoid.

\--- task \---

Add a new sprite that looks like this, and call it 'gate':

![screenshot](images/boat-gate.png)

Make sure that the colour of the gate sprite is the same as the colour of the wooden barriers.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \---

Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![gate](images/gate.png)

```blocks3
назавжди
кінець

повернути cw (1) градусів

коли прапорець натиснув
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

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