## Zwycięski!

\--- zadanie \--- Teraz dodaj kolejną instrukcję `if`{: class = "block3control"} do kodu duszka twojej łodzi, aby gracz wygrał, gdy dotrze na żółtą wyspę.

Gdy łódź dotrze na wyspę, gra powinna powiedzieć „TAK!”, A potem powinna się zakończyć.

\--- wskazówki \--- \--- wskazówka \--- Musisz dodać więcej bloków kodu w swojej `pętli na zawsze`{: class = "block3control"}, aby Twój kod sprawdzał, czy gracz wygrał:

`jeśli`{: class = "block3control"} łódź ma `dotknięcie`{: class = "block3sensing"} kolor wyspy, musisz `powiedzieć „YEAH!” na 2 sekundy`{: class = "block3looks"}, a następnie `zatrzymaj wszystkie`{: class = "block3control"}, aby zakończyć grę. \--- / wskazówka \--- \--- wskazówka \--- Oto potrzebne bloki kodu: ![duszek łodzi](images/boat_resize.png)

```blocks3
powiedz [YEAH!] przez (2) sekundy

jeśli <touching color [#FFFF99] ?> to
koniec

stop [wszystkie v]

```

\--- / wskazówka \--- \--- wskazówka \--- Oto jak powinien wyglądać twój nowy kod: ![duszek łodzi](images/boat_resize.png)

```blocks3
jeśli <touching color [#FFFF99] ?> to
powie [YEAH!] przez (2) sekundy
stop [all v]
end
```

Nie zapominaj, że ten nowy kod musi znajdować się w pętli `zawsze`{: class = "block3control"}. \--- / wskazówka \--- \--- / wskazówki \--- \--- / zadanie \---