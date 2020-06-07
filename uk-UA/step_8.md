## Перешкоди і прискорювачі

Зараз гра **занадто** легка, тож ти додаси деякі речі, щоб зробити її більш цікавою.

По-перше, ти додаси прискорювачі, щоб розганяти човен.

\--- task \---

Відредагуй тло Сцени, додавши до нього кілька білих стрілок.

![screenshot](images/boat-boost.png)

\--- /task \---

\--- task \---

Тепер додай блоки коду до циклу `завжди`{:class="block3control"}, щоб спрайт човна переміщувався на три додаткових кроки, коли торкається білої стрілки.

![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [#FFFFFF] ?> then
move (3) steps
end
```

\--- /task \---

\--- task \---

Протестуй свою гру, щоб переконатися, що твої нові стрілки-прискорювачі розганяють човен.

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
forever
end

turn cw (1) degrees

when flag clicked
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
when flag clicked
forever
turn cw (1) degrees
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---