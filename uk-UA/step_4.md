## Аварія!

На даний момент спрайт з човна може просто плисти по дерев'яних перешкодах! Тепер ви збираєтеся це виправити.

\--- task \---

Вам знадобляться два костюми для вашого спрайта на човні: один звичайний костюм, і один для того, коли човен аварії. Дублюйте костюм спрайту вашого судна, і назвіть один костюм "нормальний", а другий - "хіт".

\--- /task \---

\--- task \---

Натисніть на свій «хіт» костюм, і використовуйте **Виберіть** інструмент для захоплення частини костюма і переміщати і обертати їх , щоб зробити зовнішній вигляд човна , як він розбився на шматки.

![скріншот](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Тепер додайте код до свого човна так, щоб він зривався і розпадався, коли він торкався будь-яких коричневих дерев'яних бар'єрів.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
якщо <touching color [ ] ?> , то
кінець

перейти до х: (-190) у: (-150)

перемикача костюм , щоб (вдарив v)

точки в напрямку (0)

Перемикач костюм (з нормальною V)

говорять [Noooooo!] для (2) секунд
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
коли прапорець натиснув
в напрямку (0)
перейдіть на x: (-190) y: (-150)
назавжди
якщо <(відстань до (вказівник миші v)) > [5]> потім
напрямку (миша вказівник v)
переміщення (1) кроки
кінець
якщо <touching color [#663b00] ?> потім
перемикання костюм на (удар v)
сказати [Noooooo!] протягом (2) секунди
перейти костюм до (нормальний v)
точок у напрямку (0)
перейти до x: (-190) y: (-150)
кінець
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---