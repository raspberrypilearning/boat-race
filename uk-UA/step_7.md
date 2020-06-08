## Додавання таймера

Тепер ти додаси в свою гру таймер, щоб гравець мав діставатися до острова якомога швидше.

--- task ---

Додай нову змінну з назвою `час`{:class="block3variables"} на свою Сцену.

![знімок екрана](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Також ти можеш вибрати вигляд таймера, змінивши спосіб відображення нової змінної.

--- /task ---

--- task ---

Тепер додай блоки коду до своєї сцени, щоб таймер працював до тих пір, поки човен не досягне острова.

--- hints ---
 --- hint ---

На Сцені `коли зелений прапор натиснуто`{:class="block3control"}, `надати час значення 0`{:class="block3variables"}. Всередині свого циклу `завжди`{:class="block3control"} тобі треба спочатку `чекати 0.1 секунд`{:class="block3control"}, далі `змінити час на 0.1`{:class="block3variables"}.

--- /hint --- --- hint ---

Ось блоки коду, які тобі знадобляться:

![сцена](images/stage.png)

```blocks3
change [час v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [час v] to [0]
```

--- /hint --- --- hint ---

Ось як має виглядати твій новий код:

![сцена](images/stage.png)

```blocks3
when flag clicked
set [час v] to [0]
forever
wait (0.1) seconds
change [час v] by (0.1)
end
```

--- /hint ------ /hints ---

--- /task ---

--- task ---

Протестуй свою гру, щоб побачити, як швидко ти зможеш провести човен до острова!

![знімок екрана](images/boat-variable-test.png)

--- /task ---