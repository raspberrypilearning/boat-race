## Przeszkody i przyspieszacze

W tym momencie gra jest **zbyt** łatwa, więc dodasz kilka rzeczy, aby uczynić ją bardziej interesującą.

Najpierw dodasz kilka przyspieszaczy, aby przyspieszyć łódź.

\--- task \---

Edytuj tło sceny, dodając białe strzałki przyspieszające.

![zrzut ekranu](images/boat-boost.png)

\--- /task \---

\--- task \---

Teraz dodaj więcej bloków kodu do `pętli zawsze`{:class="block3control"}, aby duszek łodzi poruszał się o trzy dodatkowe kroki, gdy dotknie białej strzałki. ![duszek łodzi](images/boat_resize.png)

```blocks3
jeżeli <touching color [#FFFFFF] ?> to
przesuń o (3) kroki
koniec
```

\--- /task \---

\--- task \---

Przetestuj grę, aby zobaczyć, czy nowe strzałki przyspieszające przyspieszają łódź.

\--- /task \---

Następnie dodasz obrotową bramę, której łódź musi unikać.

\--- task \---

Dodaj nowego duszka, który wygląda tak, i nazwij go „brama”:

![zrzut ekranu](images/boat-gate.png)

Upewnij się, że kolor duszka bramy jest taki sam jak kolor drewnianych barier.

\--- /task \---

\--- task \---

Upewnij się, że środek duszka bramy jest ustawiony pośrodku.

![zrzut ekranu](images/boat-center.png)

\--- /task \---

\--- task \---

Dodaj kod do duszka bramy, aby obracał się powoli na zawsze.

\--- wskazówki \--- \--- wskazówka \--- Dodaj bloki kodu do duszka bramy, aby `obrócił się o 1 stopień`{:class="block3motion"} `zawsze`{:class="block3control"}. \--- /wskazówka \--- \--- wskazówka \--- Oto potrzebne bloki kodu: ![brama](images/gate.png)

```blocks3
zawsze
koniec

obróć cw o (1) stopnie

kiedy flaga kliknięta
```

\--- / wskazówka \--- \--- wskazówka \--- Oto jak powinien wyglądać twój nowy kod: ![brama](images/gate.png)

```blocks3
kiedy flaga kliknięta
zawsze
obróć cw o (1) stopni
koniec
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Sprawdź swoją grę jeszcze raz. Powinnaś teraz mieć obrotową bramę, którą musisz opłynąć swoją łodzią.

![zrzut ekranu](images/boat-gate-test.png)

\--- /task \---