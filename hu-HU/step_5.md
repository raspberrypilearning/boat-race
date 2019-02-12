## Nyerő!

\--- task \--- Most adjon még egy `ha`{: class = "block3control"} nyilatkozatot a hajó sprite kódjához, hogy a játékos nyerjen, amikor a hajót megérkezik a sárga szigetre.

Amikor a hajó eljut a szigetre, a játéknak azt kell mondania, hogy "YEAH!"

\--- hints \--- \--- hint \--- További kódblokkokat kell hozzáadnia a `forever`{: class = "block3control"} hurokhoz úgy, hogy a kódja ellenőrizze, hogy a játékos nyerte:

`, ha`{: class = "block3control"} A hajó `megható`{: class = "block3sensing"} színe a szigeten, meg kell `mondják: 'Igen!' 2 másodpercig`{: class = "block3looks"}, majd `megáll az összes`{: class = "block3control"} játék befejezéséhez. \--- / tipp \--- \--- tipp \--- Íme a szükséges kódblokkok: ![csónak-sprite](images/boat_resize.png)

```blocks3
mondjuk [YEAH!] (2) másodpercig

ha <touching color [#FFFF99] ?> majd
vég

megáll [all v]

```

\--- / tipp \--- \--- tipp \--- Íme az új kódod: ![csónak-sprite](images/boat_resize.png)

```blocks3
ha <touching color [#FFFF99] ?> akkor
mondjuk [YEAH!] (2) másodpercig
stop [all v]
vég
```

Ne feledje, hogy ez az új kód a `forever`{: class = "block3control"} hurok belsejében kell lennie. \--- / tipp \--- \--- / hints \--- \--- / feladat \---