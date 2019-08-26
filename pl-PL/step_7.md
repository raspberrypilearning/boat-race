## Dodawanie stopera

Teraz dodasz stoper do swojej gry, aby gracz musiał jak najszybciej dotrzeć na wyspę.

\--- task \---

Dodaj nową zmienną o nazwie `czas`{:class="block3variables"} do swojej Sceny.

![zrzut ekranu](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Możesz także wybrać wygląd stopera, zmieniając sposób wyświetlania nowej zmiennej.

\--- /task \---

\--- task \---

Teraz dodaj bloki kodu do swojej Sceny, aby stoper odliczał czas, aż łódź dotrze na wyspę.

\--- wskazówki \--- \--- wskazówka \--- Na Scenie, `gdy zielona flaga zostanie kliknięta`{:class="block3control"}, `ustaw czas na 0`{:class="block3variables"}. Wewnątrz `pętli zawsze`{:class="block3control"} musisz najpierw `poczekać 0.1 sekund`{:class="block3control"}, a następnie `zmienić czas o 0.1`{:class="block3variables"}. \--- / podpowiedź \--- \--- podpowiedź \--- Oto bloki kodu, których potrzebujesz: ![scena](images/stage.png)

```blocks3
zmień [czas v] o (0.1)

gdy flaga kliknięta

zawsze
koniec

czekaj (0.1) sekund

ustaw [czas v] na [0]
```

\--- / wskazówka \--- \--- wskazówka \--- Oto jak powinien wyglądać twój nowy kod: ![scena](images/stage.png)

```blocks3
gdy flaga kliknięta
ustaw [czas v] na [0]
zawsze
czekaj (0.1) sekund
zmień [czas v] o (0.1)
koniec
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Sprawdź swoją grę i przekonaj się, jak szybko uda ci się dotrzeć na wyspę!

![zrzut ekranu](images/boat-variable-test.png)

\--- /task \---