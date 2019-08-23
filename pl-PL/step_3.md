## Sterowanie łodzią

Gracz kontroluje duszka łodzi za pomocą myszy.

\--- zadanie \--- Dodaj kod do duszka łodzi, aby zaczynał się w lewym dolnym rogu, wskazując w górę, a następnie podążał za wskaźnikiem myszy.

![duszek łodzi](images/boat_resize.png)

```blocks3
po kliknięciu flagi
punkt w kierunku (0)
przejdź do x: (-190) y: (-150)
zawsze
punkt w kierunku (wskaźnik myszy v)
ruchy (1) kroki
```

\--- /task \---

\--- task \---

**Przetestuj kod** , klikając zieloną flagę i poruszając myszą. Czy duszek łodzi przesuwa się w kierunku wskaźnika myszy?

![zrzut ekranu](images/boat-mouse.png)

\--- brak wydruku \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- / brak wydruku \---

\--- tylko do drukowania \--- ![screenshot](images/boat-pointer-test-anim.png) \--- /tylko do drukowania \---

\--- /task \---

\--- task \---

Co się stanie, gdy łódź osiągnie wskaźnik myszy? Wypróbuj, aby zobaczyć, na czym polega problem.

\--- /task \---

\--- task \---

Aby temu zapobiec, musisz dodać do kodu blok `jeżeli`{:class="block3control"}, aby duszek łodzi poruszał się tylko wtedy, gdy jest więcej niż 5 pikseli od wskaźnika myszy.

\--- wskazówki \--- \--- wskazówka \--- Łódź powinna wskazywać tylko wskaźnik myszy i przesuwać `jeśli`{: class = "block3control"} `odległość od wskaźnika myszy`{: class = „block3sensing”} jest większy o `niż 5 pikseli`{: class = "block3operators"}. \--- / wskazówka \--- \--- wskazówka \--- Oto bloki kodu, które należy dodać do kodu duszka łodzi: ![duszek łodzi](images/boat_resize.png)

```blocks3
jeśli < [] > [] > to

(odległość do (wskaźnik myszy v))
```

\--- /hint \--- \--- hint \--- Twój kod powinien wyglądać tak: ![duszek łodzi](images/boat_resize.png)

```blocks3
po kliknięciu flagi
punkt w kierunku (0)
przejdź do x: (-190) y: (-150)
zawsze
jeśli <(odległość do (wskaźnik myszy v)) > [5]> a następnie
punktów w kierunku (mysz- wskaźnik v)
ruchów (1) kroków
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Przetestuj kod ponownie, aby sprawdzić, czy problem został już rozwiązany.

\--- /task \---