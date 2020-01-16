## Додати таймер

Тепер у вашу гру буде додано таймер, щоб гравець якомога швидше дістався до острова.

\--- task \---

Додайте нову змінну, що називається `time`{: class = "block3variables"} на ваш етап.

![скріншот](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Ви також можете вибрати вигляд таймера, змінивши спосіб відображення нової змінної.

\--- /task \---

\--- task \---

Тепер додайте кодові блоки до вашої Stage, щоб таймер підраховував до тих пір, поки човен не досягне острова.

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
змінити [час v] на (0,1)

коли прапор натиснув

назавжди
кінець

чекати (0,1) секунди

встановити [час від] до [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
коли прапорець натиснув
встановити [час v] на [0]
назавжди
чекати (0,1) секунди
змінити [час v] на (0,1)
кінець
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---