## Dodawanie timera

Teraz dodasz licznik do swojej gry, aby gracz musiał jak najszybciej dotrzeć na wyspę.

\--- task \---

Dodaj nową zmienną o nazwie `time`{: class = "block3variables"} na stole montażowym.

![zrzut ekranu](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Możesz także wybrać wygląd timera, zmieniając sposób wyświetlania nowej zmiennej.

\--- /task \---

\--- task \---

Teraz dodaj bloki kodu do stołu montażowego, aby licznik odliczał czas, aż łódź dotrze na wyspę.

\--- wskazówki \--- \--- wskazówka \--- Na stole montażowym, `po kliknięciu zielonej flagi`{: class = "block3control"}, `ustaw czas na 0`{: class = "block3variables „}. Wewnątrz `zawsze`pętli {: class = "block3control"} musisz najpierw `poczekać 0,1 sek.`{: class = "block3control"}, a następnie `zmienić czas o 0,1`{: class = "block3variables" }. \--- / podpowiedź \--- \--- podpowiedź \--- Oto bloki kodu, których potrzebujesz: ![etap](images/stage.png)

```blocks3
zmień [czas v] o (0,1)

po kliknięciu flagi

zawsze
koniec

poczekaj (0,1) sekund

ustaw [czas v] na [0]
```

\--- / wskazówka \--- \--- wskazówka \--- Oto jak powinien wyglądać twój nowy kod: ![etap](images/stage.png)

```blocks3
po kliknięciu flagi
ustaw [czas v] na [0]
zawsze
poczekaj (0,1) sekundy
zmień [czas v] o (0,1)
koniec
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Sprawdź swoją grę i przekonaj się, jak szybko uda ci się dotrzeć na wyspę!

![zrzut ekranu](images/boat-variable-test.png)

\--- /task \---