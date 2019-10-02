## Upravljanje čolna

Igralec bo čoln upravljal z miško.

\--- task \--- Figuri čolna dodaj kodo, da bo čoln startal v spodnjem levem kotu, obrnjen navzgor, potem pa bo sledil kazalcu miške.

![čoln](images/boat_resize.png)

```blocks3
ko kliknemo na zastavico
obrni se v smer (0)
pojdi na x: (-190) y: (-150)
ponavljaj
obrni se proti (kazalcu miške v)
pojdi (1) korakov
```

\--- /task \---

\--- task \---

**Preveri svojo kodo** s klikom na zeleno zastavico in premikanjem miške. Ali se figura ladje premakne proti miškinemu kazalcu?

![posnetek zaslona](images/boat-mouse.png)

\--- no-print \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- /no-print \---

\--- print-only \--- ![screenshot](images/boat-pointer-test-anim.png) \--- /print-only \---

\--- /task \---

\--- task \---

Kaj se zgodi, ko čoln doseže kazalec miške? Preizkusi, da vidiš v čem je težava.

\--- /task \---

\--- task \---

Da se to ne bi več dogajalo, moraš dodati `če`{: class = "block3control"} blok v tvojo kodo, da se bo figura čolna premikala le, če je oddaljena več kot 5 pikslov od kazalca miške.

\--- hints \--- \--- hint \--- Čoln naj bo obrnjen le proti kazalcu miške in naj se premika, `če`{:class="block3control"} je `razdalja do kazalca miške`{:class="block3sensing"} `večja od 5 pikslov`{:class="block3operators"}. \--- /hint \--- \--- hint \--- To so bloki kode, ki jih moraš dodsti kodi figure čolna: ![čoln](images/boat_resize.png)

```blocks3
če < [] > [] > potem

(razdalja do (kazalca miške v))
```

\--- /hint \--- \--- hint \--- Tvoja koda bi morala izgledati tako: ![čoln](images/boat_resize.png)

```blocks3
ko kliknemo na zastavico
obrni se v smer (0)
pojdi na x: (-190) y: (-150)
ponavljaj
če <(razdalja do (kazalca miške v)) > [5]> potem
obrni se proti (kazalcu miške v)
pojdi (1) korakov
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Ponovno preizkusi svojo kodo in preveri ali je težava odpravljena.

\--- /task \---