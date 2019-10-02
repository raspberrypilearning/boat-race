## Wygrana!

--- task --- Teraz dodaj kolejną instrukcję `jeżeli`{:class="block3control"} do kodu duszka twojej łodzi, aby gracz wygrał, gdy dotrze na żółtą wyspę.

Gdy łódź dotrze na wyspę, gra powinna powiedzieć „TAK!”, a potem powinna się zakończyć.

--- hints ---
 --- hint --- Musisz dodać więcej bloków kodu w swojej pętli `zawsze`{:class="block3control"}, aby Twój kod sprawdzał, czy gracz wygrał:

`jeżeli`{:class="block3control"} łódź `dotyka`{:class="block3sensing"} kolor wyspy, musisz `powiedzieć „TAK!” przez 2 sekundy`{:class="block3looks"}, a następnie `zatrzymaj wszystkie`{:class="block3control"}, aby zakończyć grę.
--- /hint ---
 --- hint --- Oto potrzebne bloki kodu: ![duszek łodzi](images/boat_resize.png)

```blocks3
powiedz [TAK!] przez (2) sekund

jeżeli <dotyka koloru [#FFFF99] ?> to
koniec

zatrzymaj [wszystkie v]

```

--- /hint --- --- hint --- Oto jak powinien wyglądać twój nowy kod: ![duszek łodzi](images/boat_resize.png)

```blocks3
jeżeli <dotyka koloru [#FFFF99] ?> to
powiedz [TAK!] przez (2) sekund
zatrzymaj [wszystkie v]
koniec
```

Nie zapominaj, że ten nowy kod musi znajdować się w pętli `zawsze`{:class="block3control"}.
--- /hint ---
--- /hints --- --- /task ---