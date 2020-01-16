## Dodawanie stopera

Teraz dodasz stoper do swojej gry, aby gracz musiał dotrzeć na wyspę najszybciej jak to możliwe.

\--- task \---

Dodaj nową zmienną o nazwie `czas`{:class="block3variables"} do swojej Sceny.

![zrzut ekranu](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Możesz także wybrać wygląd stopera, zmieniając sposób wyświetlania nowej zmiennej.

\--- /task \---

\--- task \---

Teraz dodaj bloki kodu do swojej Sceny, aby stoper odliczał czas, aż łódź dotrze na wyspę.

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
zmień [czas v] o (0.1)

kiedy kliknięto zieloną flagę

zawsze
koniec

czekaj (0.1) sekund

ustaw [czas v] na [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
kiedy kliknięto zieloną flagę
ustaw [czas v] na [0]
zawsze
czekaj (0.1) sekund
zmień [czas v] o (0.1)
koniec
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---