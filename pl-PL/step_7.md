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

Na scenie, `kiedy kliknięto zieloną flagę`{:class="block3control"}, `ustaw czas na 0`{:class="block3variables"}. Wewnątrz pętli `zawsze`{:class="block3control"} musisz najpierw `czekać 0.1 sekund`{:class="block3control"}, a następnie `zmienić czas o 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Oto potrzebne bloki kodu:

![scena](images/stage.png)

```blocks3
change [time v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [time v] to [0]
```

\--- /hint \--- \--- hint \---

Tak powinien wyglądać Twój kod:

![scena](images/stage.png)

```blocks3
when flag clicked
set [time v] to [0]
forever
wait (0.1) seconds
change [time v] by (0.1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Sprawdź swoją grę i przekonaj się, jak szybko uda ci się dotrzeć na wyspę!

![zrzut ekranu](images/boat-variable-test.png)

\--- /task \---