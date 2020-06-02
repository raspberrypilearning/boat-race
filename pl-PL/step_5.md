## Wygrana!

\--- task \---

Teraz dodaj kolejną instrukcję `jeżeli`{:class="block3control"} do kodu duszka twojej łodzi, aby gracz wygrał, gdy dotrze na żółtą wyspę.

Gdy łódź dotrze na wyspę, gra powinna powiedzieć „TAK!”, a potem powinna się zakończyć.

\--- hints \--- \--- hint \---

Musisz dodać więcej bloków kodu w swojej pętli `zawsze`{:class="block3control"}, aby Twój kod sprawdzał, czy gracz wygrał:

`jeżeli`{:class="block3control"} łódź `dotyka`{:class="block3sensing"} kolor wyspy, musisz `powiedzieć „TAK!” przez 2 sekundy`{:class="block3looks"}, a następnie `zatrzymaj wszystkie`{:class="block3control"}, aby zakończyć grę.

\--- /hint \--- \--- hint \---

Oto potrzebne bloki kodu:

![duszek łodzi](images/boat_resize.png)

```blocks3
say [YEAH!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

\--- /hint \--- \--- hint \---

Tak powinien wyglądać Twój kod:

![duszek łodzi](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
```

Nie zapominaj, że ten nowy kod musi znajdować się w pętli `zawsze`{:class="block3control"}.

\--- /hint \--- \--- /hints \--- \--- /task \---