## Sterowanie łodzią

Gracz kontroluje duszka łodzi za pomocą myszy.

\--- zadanie \--- Dodaj kod do duszka łodzi, aby zaczynał się w lewym dolnym rogu, wskazując w górę, a następnie podążał za wskaźnikiem myszy.

![duszek łodzi](images/boat_resize.png)

```blocks3
gdy flaga kliknięta
ustaw kierunek na (0)
przejdź do x: (-190) y: (-150)
zawsze
ustaw w kierunku duszka (wskaźnik myszy v)
przesuń o (1) kroki
```

\--- /task \---

\--- task \---

**Przetestuj swój kod**, klikając zieloną flagę i poruszając myszą. Czy duszek łodzi przesuwa się w kierunku wskaźnika myszy?

![zrzut ekranu](images/boat-mouse.png)

\--- brak wydruku \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- / brak wydruku \---

\--- tylko do drukowania \--- ![screenshot](images/boat-pointer-test-anim.png) \--- /tylko do drukowania \---

\--- /task \---

\--- task \---

Co się stanie, gdy łódź dopłynie do wskaźnika myszy? Wypróbuj, aby zobaczyć, na czym polega problem.

\--- /task \---

\--- task \---

Aby temu zapobiec, musisz dodać do kodu blok `jeżeli`{:class="block3control"}, aby duszek łodzi poruszał się tylko wtedy, gdy jest więcej niż 5 pikseli od wskaźnika myszy.

\--- wskazówki \--- \--- wskazówka \--- Łódź powinna wskazywać w kierunku wskaźnika myszy i przesuwać się `jeśli`{:class="block3control"} `odległość od wskaźnika myszy`{:class=„block3sensing”} jest `większa niż 5 pikseli`{:class="block3operators"}. \--- /wskazówka \--- \--- wskazówka \--- Oto bloki kodu, które należy dodać do kodu duszka łodzi: ![duszek łodzi](images/boat_resize.png)

```blocks3
jeżeli < [] > [] > to

(odległość do (wskaźnik myszy v))
```

\--- /hint \--- \--- hint \--- Twój kod powinien wyglądać tak: ![duszek łodzi](images/boat_resize.png)

```blocks3
kiedy flaga kliknięta
ustaw kierunek na (0)
przejdź do x: (-190) y: (-150)
zawsze
jeżeli <(odległość do (wskaźnik myszy v)) > [5]> to
ustaw w kierunku duszka (mysz- wskaźnik v)
przesuń o (1) kroków
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Przetestuj swój kod ponownie, aby sprawdzić, czy problem został już rozwiązany.

\--- /task \---