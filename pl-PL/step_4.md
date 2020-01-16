## Zderzenia!

W tej chwili duszek łodzi może po prostu żeglować przez drewniane bariery! Teraz to naprawisz.

\--- task \---

Potrzebujesz dwa kostiumy dla duszka łodzi: jeden normalny kostium i jeden na wypadek uderzenia łodzi. Zduplikuj kostium duszka łodzi i nazwij jeden kostium „normalny”, a drugi „po uderzeniu”.

\--- /task \---

\--- task \---

Kliknij kostium „po uderzeniu” i użyj narzędzia **Wybierz**, aby chwycić części kostiumu, przesuwać je i obracać, aby łódź wyglądała, jakby się rozbiła.

![zrzut ekranu](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Teraz dodaj kod do swojej łodzi, aby rozbiła się i rozpadła, gdy dotknie jakiejkolwiek brązowej drewnianej bariery.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
jeżeli < dotyka koloru [kolor] ? > to
koniec

idź do x: (-190) y: (-150)

zmień kostium na (po uderzeniu v)

ustaw kierunek na (0)

przełącz kostium na (normalny v)

powiedz [Nieeee!] przez (2) sekund
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
kiedy kliknięto zieloną flagę
ustaw kierunek na (0)
idź do x: (-190) y: (-150)
zawsze
jeżeli <(odległość od (wskaźnik myszy v)) > [5]> to
ustaw w kierunku duszka (wskaźnik myszy v)
przesuń o (1) kroki
koniec
jeżeli <dotyka koloru [#663b00] ?> to
zmień kostium na (po uderzeniu v)
powiedz [Nieeee!] przez (2) sekund
przełącz kostium na (normalny v)
ustaw kierunek na (0)
idź do x: (-190) y: (-150)
koniec
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---