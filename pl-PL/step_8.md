## Przeszkody i przyspieszacze

W tym momencie gra jest **zbyt** łatwa, więc dodasz kilka rzeczy, aby uczynić ją bardziej interesującą.

Najpierw dodasz kilka przyspieszaczy, aby przyspieszyć łódź.

\--- task \---

Edytuj tło sceny, dodając białe strzałki przyspieszające.

![zrzut ekranu](images/boat-boost.png)

\--- /task \---

\--- task \---

Teraz dodaj więcej bloków kodu do pętli `zawsze`{:class="block3control"}, aby duszek łodzi poruszał się o trzy dodatkowe kroki, gdy dotknie białej strzałki. ![duszek łodzi](images/boat_resize.png)

```blocks3
jeżeli < dotyka koloru [#Ffffff] ?> to
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

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![brama](images/gate.png)

```blocks3
zawsze
koniec

obróć w prawo o (1) stopni

kiedy kliknięto zieloną flagę
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

```blocks3
kiedy kliknięto zieloną flagę
zawsze
obróć w prawo o (1) stopni
koniec
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---