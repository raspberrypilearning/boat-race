## Nadziranje čolna

Igralec bo upravljal čarovnik z miško.

\--- naloga \--- Dodajte kodo v žig čolna, tako da se začne v spodnjem levem kotu obrnjenega navzgor in nato sledi kazalcu miške.

![čoln](images/boat_resize.png)

```blocks3
ko je zastavica kliknila
v smeri (0)
pojdi na x: (-190) y: (-150)
vedno
točke proti (kazalec miške v)
premakni (1) korake
```

\--- /task \---

\--- task \---

**Preverite svojo kodo** s klikom na zeleno zastavo in premikanjem miške. Ali se žig ladje premakne proti kazalcu miške?

![posnetek zaslona](images/boat-mouse.png)

\--- no-print \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- / brez tiskanja \---

\--- samo za tiskanje \--- ![screenshot](images/boat-pointer-test-anim.png) \--- / samo za tiskanje \---

\--- /task \---

\--- task \---

Kaj se zgodi, ko čoln doseže kazalec miške? Preizkusite, da vidite, v čem je težava.

\--- /task \---

\--- task \---

Da bi to preprečili zgodilo, morate dodaj `ali`{: class = "block3control"} blok v kodo, tako da Sprite čoln premika le, če je več kot 5 pik od kazalca miške.

\--- namigi \--- \--- namig \--- Čoln mora samo kazati proti kazalcu miške in se premakniti `če`{: class = "block3control"} `razdalje do kazalca miške`{: class = "block3sensing"} je `več kot 5 pikslov`{: class = "block3operators"}. \--- / namig \--- \--- namig \--- To so kodni bloki, ki jih morate dodati kodi za čarovniški duh: ![čoln](images/boat_resize.png)

```blocks3
če < [] > [] > potem

(razdalja do (kazalec miške v))
```

\--- / namig \--- \--- namig \--- To je tisto, kar mora izgledati vaša koda: ![čoln](images/boat_resize.png)

```blocks3
ko je zastavica kliknila
točko v smeri (0)
pojdite na x: (-190) y: (-150)
vedno
če <(razdalja do (kazalec miške v)) > [5]> in
proti (miška kazalec v)
premikanje (1) korakov
```

\--- / namig \--- \--- / namigi \---

\--- /task \---

\--- task \---

Ponovno preizkusite svojo kodo, da preverite, ali je težava odpravljena.

\--- /task \---