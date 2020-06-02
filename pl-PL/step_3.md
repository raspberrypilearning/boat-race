## Sterowanie łodzią

Gracz będzie kontrolować duszka łodzi za pomocą myszy.

\--- task \---

Dodaj kod do duszka łodzi, aby pojawiał się w lewym dolnym rogu, wskazując w górę, a następnie podążał za wskaźnikiem myszy.

![duszek łodzi](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
point towards (mouse-pointer v)
move (1) steps
```

\--- /task \---

\--- task \---

**Przetestuj swój kod**, klikając zieloną flagę i poruszając myszą. Czy duszek łodzi przesuwa się w kierunku wskaźnika myszy?

![zrzut ekranu](images/boat-mouse.png)

\--- no-print \---

![zrzut ekranu](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![zrzut ekranu](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

Co się stanie, gdy łódź dopłynie do wskaźnika myszy? Wypróbuj, aby zobaczyć, na czym polega problem.

\--- /task \---

\--- task \---

Aby temu zapobiec, musisz dodać do kodu blok `jeżeli`{:class="block3control"}, aby duszek łodzi poruszał się tylko wtedy, gdy jest więcej niż 5 pikseli od wskaźnika myszy.

\--- hints \--- \--- hint \---

Łódź powinna wskazywać w kierunku wskaźnika myszy i przesuwać się `jeżeli`{:class="block3control"} `odległość od wskaźnika myszy`{:class=„block3sensing”} jest `większa niż 5 pikseli`{:class="block3operators"}.

\--- /hint \--- \--- hint \---

Oto bloki kodu, które należy dodać do kodu duszka łodzi:

![duszek łodzi](images/boat_resize.png)

```blocks3
if < [ ] > [ ] > then

(distance to (mouse-pointer v))
```

\--- /hint \--- \--- hint \---

Tak powinien wyglądać Twój kod:

![duszek łodzi](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Przetestuj swój kod ponownie, aby sprawdzić, czy problem został już rozwiązany.

\--- /task \---