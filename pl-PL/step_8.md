## Przeszkody i przyspieszacze

W tym momencie gra jest **zbyt** łatwa, więc dodasz kilka rzeczy, aby uczynić ją bardziej interesującą.

Najpierw dodasz kilka przyspieszaczy, aby przyspieszyć łódź.

--- task ---

Edytuj tło sceny, dodając białe strzałki przyspieszające.

![zrzut ekranu](images/boat-boost.png)

--- /task ---

--- task ---

Teraz dodaj więcej bloków kodu do pętli `zawsze`{:class="block3control"}, aby duszek łodzi poruszał się o trzy dodatkowe kroki, gdy dotknie białej strzałki. ![duszek łodzi](images/boat_resize.png)

```blocks3
jeżeli < dotyka koloru [#Ffffff] ?> to
przesuń o (3) kroków
koniec
```

--- /task ---

--- task ---

Przetestuj grę, aby zobaczyć, czy nowe strzałki przyspieszające przyspieszają łódź.

--- /task ---

Następnie dodasz obrotową bramę, której łódź musi unikać.

--- task ---

Dodaj nowego duszka, który wygląda tak, i nazwij go „brama”:

![zrzut ekranu](images/boat-gate.png)

Upewnij się, że kolor duszka bramy jest taki sam jak kolor drewnianych barier.

![zrzut ekranu](images/brown-hsv.png)

--- /task ---

--- task ---

Upewnij się, że środek duszka bramy jest ustawiony pośrodku.

![zrzut ekranu](images/boat-center.png)

--- /task ---

--- task ---

Dodaj kod do duszka bramy, aby obracał się powoli w nieskończoność.

--- hints ---
 --- hint --- Dodaj bloki kodu do duszka bramy, aby `obrócił się o 1 stopień`{:class="block3motion"} `zawsze`{:class="block3control"}.
--- /hint ---
 --- hint --- Oto potrzebne bloki kodu: ![brama](images/gate.png)

```blocks3
zawsze
koniec

obróć w prawo o (1) stopni

kiedy kliknięto zieloną flagę
```

--- /hint --- --- hint --- Oto jak powinien wyglądać twój nowy kod: ![brama](images/gate.png)

```blocks3
kiedy kliknięto zieloną flagę
zawsze
obróć w prawo o (1) stopni
koniec
```

--- /hint --- --- /hints ---

--- /task ---

--- task ---

Sprawdź swoją grę jeszcze raz. Powinnaś teraz mieć obrotową bramę, którą musisz opłynąć swoją łodzią.

![zrzut ekranu](images/boat-gate-test.png)

--- /task ---