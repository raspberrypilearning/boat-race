## Аварія!

Зараз спрайт човна може просто пропливати крізь дерев'яні перешкоди! Тепер ти це виправиш.

\--- task \---

Тобі знадобляться два образи для свого спрайта човна: один звичайний і один для човна після аварії. Продублюй образ човна, після чого назви один з них "нормальний", а другий — "розбитий".

\--- /task \---

\--- task \---

Клацни на свій образ "розбитий" і використай інструмент **Обрати** для переносу та повороту частин образу, щоб виглядало так, ніби човен розбився на шматки.

![screenshot](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Тепер додай код до свого човна, щоб він врізався і розпадався, коли торкався будь-яких коричневих дерев'яних перешкод.

\--- hints \--- \--- hint \---

Тобі треба додати блоки коду всередині свого циклу `завжди`{:class="block3control"}, щоб твій код постійно перевіряв, чи спрайт човна не врізався, та якщо це трапляється, то потрібно відновити початкову позицію спрайта човна.

`Якщо`{:class="block3control"} човен `торкається`{:class="block3sensing"} коричневого кольору, тобі треба `змінити образ на "розбитий"`{:class="block3looks"}, `говорити "Ні-і-і-і-і!" 2 секунди`{:class="block3looks"}, а потім `змінити образ на "звичайний"`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [ ] ?> then
end

go to x: (-190) y: (-150)

switch costume to (hit v)

point in direction (0)

switch costume to (normal v)

say [Noooooo!] for (2) seconds
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
end
if <touching color [#663b00] ?> then
switch costume to (hit v)
say [Noooooo!] for (2) seconds
switch costume to (normal v)
point in direction (0)
go to x: (-190) y: (-150)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---