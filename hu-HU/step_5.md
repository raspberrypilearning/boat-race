## Győzelem!

\--- task \--- Most adj hozzá egy újabb `ha`{:class="block3control"} utasítást a hajó szereplőd kódjához, hogy a játékos nyerjen, ha sikerül elvezetnie a hajót a sárga szigetre.

Amikor a hajó eljut a szigetre, a játéknak azt kell mondania, hogy "IGEN!", aztán be kell fejeződnie.

\--- hints \--- \--- hint \--- További kódblokkokat kell hozzáadnod a `mindig`{: class = "block3control"} ciklushoz úgy, hogy a kódod folyamatosan ellenőrizze, hogy a játékos nyert-e:

`Ha`{:class="block3control"} a hajó `érinti`{:class="block3sensing"} a színét, azt kell `mondanod, hogy 'IGEN!' 2 másodpercig`{:class="block3looks"} majd `álljon le minden feladat`{:class="block3control"}, hogy a játék befejeződjön. \--- /hint \--- \--- hint \--- Íme a szükséges kódblokkok: ![hajó szereplő](images/boat_resize.png)

```blocks3
mondd: [IGEN!] (2) másodpercig

ha <touching color [#FFFF99] ?> akkor
end

álljon le [minden feladat v]

```

\--- /hint \--- \--- hint \--- Így kell kinéznie a kódodnak: ![hajó szereplő](images/boat_resize.png)

```blocks3
ha <touching color [#FFFF99] ?> akkor 
  mondd: [IGEN!] (2) másodpercig
  álljon le [minden feladat v]
end
```

Ne feledd, hogy ezt az új kódot a `mindig`{:class="block3control"} cikluson belülre kell raknod. \--- /hint \--- \--- /hints \--- \--- /task \---