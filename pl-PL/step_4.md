## Zderzenia!

W tej chwili duszek łodzi może po prostu żeglować przez drewniane bariery! Naprawisz to teraz.

\--- task \---

Potrzebujesz dwa kostiumy dla duszka łodzi: jeden normalny kostium i jeden na wypadek uderzenia łodzi. Zduplikuj kostium duszka łodzi i nazwij jeden kostium „normalny”, a drugi „po uderzeniu”.

\--- /task \---

\--- task \---

Kliknij kostium „po uderzeniu” i użyj narzędzia **Wybierz**, aby chwycić części kostiumu, przesuwać je i obracać, aby łódź wyglądała, jakby się rozbiła.

![zrzut ekranu](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Teraz dodaj kod do swojej łodzi, aby rozbiła się i rozpadła, gdy dotknie jakiejkolwiek brązowej drewnianej bariery.

\--- wskazówki \--- \--- wskazówka \--- Musisz dodać bloki kodu do swojej pętli `zawsze`{:class="block3control"}, aby Twój kod sprawdzał, czy duszek łodzi się rozbił, i jeśli się rozbił, kod musi zresetować pozycję duszka łodzi.

`jeżeli`{:class="block3control"} łódź `dotyka`{:class="block3sensing"} brązowy kolor drewna, musisz `przełączyć na kostium "po uderzeniu"`{:class="block3looks"}, `powiedz Nieee! przez 2 sekundy`{:class="block3looks"}, a następnie `przełącz się z powrotem na kostium "normalny"`{:class="block3looks"}. Na koniec musisz `skierować w górę`{:class="block3motion"} i `przejść do pozycji początkowej`{:class="block3motion"}.

\--- /hint \--- \--- hint \--- Oto potrzebne bloki kodu: ![duszek łodzi](images/boat_resize.png)

```blocks3
jeżeli <touching color [ ] ?> to
koniec

idź do x: (-190) y: (-150)

zmień kostium na (po uderzeniu v)

ustaw na kierunek (0)

przełącz kostium na (normalny v)

powiedz [Nieeee!] przez (2) sekundy
```

\--- / wskazówka \--- \--- wskazówka \--- Oto jak powinien wyglądać twój kod: ![duszek łodzi](images/boat_resize.png)

```blocks3
gdy flaga kliknięta
ustaw kierunek na (0)
idź do x: (-190) y: (-150)
zawsze
jeżeli <(odległość do (wskaźnik myszy v)) > [5]> to
ustaw w kierunku duszka (mysz- wskaźnik v)
przesuń o (1) kroki
koniec
jeżeli <touching color [#663b00] ?> to
zmień kostium na (po uderzeniu v)
powiedz [Nieeee!] przez (2) sekundy
przełącz kostium na (normalny v)
ustaw na kierunek (0)
idź do x: (-190) y: (-150)
koniec
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Powinieneś także dodać kod, aby upewnić się, że twój duszek zawsze rozpoczyna z "normalnym" wyglądem „normalnie”.

Sprawdź swój kod ponownie. Jeśli teraz spróbujesz przepłynąć łodzią przez drewnianą barierę, łódź powinna się rozbić, a następnie powrócić do pozycji wyjściowej.

![zrzut ekranu](images/boat-crash.png)

\--- /task \---