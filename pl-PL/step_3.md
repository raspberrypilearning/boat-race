## Sterowanie łodzią

Gracz będzie kontrolować duszka łodzi za pomocą myszy.

--- task --- Dodaj kod do duszka łodzi, aby pojawiał się w lewym dolnym rogu, wskazując w górę, a następnie podążał za wskaźnikiem myszy.

![duszek łodzi](images/boat_resize.png)

```blocks3
kiedy kliknięto zieloną flagę
ustaw kierunek na (0)
Idź do x: (-190) y: (-150)
zawsze 
ustaw w kierunku duszka (wskaźnik myszy v)
przesuń o (1) kroków
end
```

--- /task ---

--- task ---

**Przetestuj swój kod**, klikając zieloną flagę i poruszając myszą. Czy duszek łodzi przesuwa się w kierunku wskaźnika myszy?

![zrzut ekranu](images/boat-mouse.png)

--- no-print ---
![zrzut ekranu](images/boat-pointer-test-anim.gif)
--- /no-print ---

--- print-only ---
![zrzut ekranu](images/boat-pointer-test-anim.png)
--- /print-only ---

--- /task ---

--- task ---

Co się stanie, gdy łódź dopłynie do wskaźnika myszy? Wypróbuj, aby zobaczyć, na czym polega problem.

--- /task ---

--- task ---

Aby temu zapobiec, musisz dodać do kodu blok `jeżeli`{:class="block3control"}, aby duszek łodzi poruszał się tylko wtedy, gdy jest więcej niż 5 pikseli od wskaźnika myszy.

--- hints ---

 --- hint ---
 
Łódź powinna wskazywać w kierunku wskaźnika myszy i przesuwać się `jeżeli`{:class="block3control"} `odległość od wskaźnika myszy`{:class=„block3sensing”} jest `większa niż 5 pikseli`{:class="block3operators"}.
--- /hint ---
--- hint ---

Oto bloki kodu, które należy dodać do kodu duszka łodzi:
![duszek łodzi](images/boat_resize.png)

```blocks3
jeżeli < [ ] > [ ] > to

(odległość od (wskaźnik myszy v))
```

--- /hint --- --- hint ---
Twój kod powinien wyglądać tak:
![duszek łodzi](images/boat_resize.png)

```blocks3
kiedy kliknięto zieloną flagę
ustaw kierunek na (0)
Idź do x: (-190) y: (-150)
zawsze 
jeżeli <(odległość od (wskaźnik myszy v)) > [5]> to 
ustaw w kierunku duszka (wskaźnik myszy v)
przesuń o (1) kroków
end
end
```

--- /hint --- --- /hints ---

--- /task ---

--- task ---

Przetestuj swój kod ponownie, aby sprawdzić, czy problem został już rozwiązany.

--- /task ---