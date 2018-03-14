## Sterowanie łodzią

+ Będziesz sterować łodzią za pomocą swojej myszki. Dodaj kod do swojej łodzi tak, aby startowała z dolnego lewego narożnika i była skierowana do góry, a następnie, aby podążała za wskaźnikiem myszy. **Sprawdź swój kod**, aby upewnić się, że robi to, co powinien.

\--- hints \--- \--- hint \--- `Kiedy kliknięto zieloną flagę` musisz doprowadzić łódź `do pozycji początkowej` i `ustawić kierunek na górę`. Następnie łódź musi się `ustawić w stronę wskaźnika myszki` i `przesunąć o 1 krok`. Musi to powtarzać cały czas (`zawsze`).

\--- /hint \--- \--- hint \--- Oto bloki jakich będziesz potrzebować: ![screenshot](images/boat-move-blocks.png) \--- /hint \--- \--- hint \--- Tak powinien wyglądać twój kod: ![screenshot](images/boat-move-code.png) \--- /hint \--- \--- /hints \---

+ Przetestuj swoją łódź poprzez kliknięcie flagi i poruszenie myszki. Czy łódź płynie w jej kierunku?
    
    ![screenshot](images/boat-mouse.png)
    
    ![screenshot](images/boat-pointer-test-anim.gif)

## \--- collapse \---

title: Jeśli masz problemy...

## image: images/image.png

**Informacja:** Obecnie występuje błąd w Scratch, który oznacza, że twoja łódź nie może ruszyć się w kierunku wskaźnika myszy. Jeśli tak się stanie, kliknij strzałkę w `punkcie w kierunku` bloku i ponownie wybierz `wskaźnik myszy`.

![screenshot](images/boat-bug.png) \--- /collapse \---

+ Co się stanie jeśli łódź dotrze do wskaźnika myszy? Spróbuj.

+ Aby to się nie zdarzało, musisz dodać blok warunku `if` do twojego kodu, tk aby łódź poruszała się tylko jeśli jest w odległości nie większej niż 5px od myszy.

\--- hints \--- \--- hint \--- Łódź powinna wskazywać tylko na wskaźnik myszy i poruszać się `jeżeli odległość od wskaźnika` jest `większa niż 5px`. \--- /hint \--- \--- hint \--- Tutaj są bloki kodu, które będziesz musiał dodać do kodu łodzi: ![screenshot](images/boat-pointer-blocks.png) \--- /hint \--- \--- hint \--- Tak powinien wyglądać twój kod: ![screenshot](images/boat-pointer-code.png) \--- /hint \--- \--- /hints \---

+ Jeszcze raz przetestuj swoją łódź aby sprawdzić czy problem został rozwiązany.