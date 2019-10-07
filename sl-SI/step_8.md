## Ovire in pospeševalci

Trenutno je igra **mnogo** preveč enostavna, zato boš dodal še nekaj stvari, ki jo bodo naredile bolj zanimivo.

Najprej boš dodali nekaj pospeševalcev, ki bodo pohitrili čoln.

\--- task \---

Uredi ozadje odra, tako da dodaš nekaj belih pospeševalnih puščic.

![posnetek zaslona](images/boat-boost.png)

\--- /task \---

\--- task \---

Sedaj v zanko `ponavljaj`{: class = "block3control"} dodaj bloke kode, ki bodo figuro čolna pomaknili za tri dodatne korake, kadar se čoln dotakne bele puščice. ![čoln](images/boat_resize.png)

```blocks3
če <touching color [#FFFFFF] ?> potem
pojdi (3) korakov
konec
```

\--- /task \---

\--- task \---

Preizkusi igro, da vidiš, ali te nove pospeševalne puščice zares pospešijo čoln.

\--- /task \---

Zdaj boš dodal še vrstečo se zapornico, ki se je mora čoln izogibati.

\--- task \---

Dodajte novo figuro, ki izgleda takole, in jo poimenuj 'zapornica':

![posnetek zaslona](images/boat-gate.png)

Poskrbi, da je barva zapornice eneka barvi lesenih ovir.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Poskrvi, da je središče figure zapornice postavljeno na sredino.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Figuri zapornice dodaj kodo, ki jo bo neprenehoma počasi vrstela.

\--- hints \--- \--- hint \--- Dodaj bloke kode figuri zapornice, da se `obrne za 1 stopinjo`{:class="block3motion"} in to `ponavljaj`{:class="block3control"}. \--- /hint \--- \--- hint \--- To so bloki kode, ki jih potrebuješ: ![vrata](images/gate.png)

```blocks3
ponavljaj
konec

obrni se za (1) stopinj v desno

ko kliknemo na zastavico
```

\--- /hint \--- \--- hint \--- Tako bi morala izgledati tvoja koda: ![zapornica](images/gate.png)

```blocks3
ko kliknemo na zastavico
ponavljaj
obrni se za (1) stopinj v desno
konec
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Zpoet preizkusi svojo igro. Zdaj bi morala imeti vrtečo se zapornico, okoli katere moraš pripeljati svoj čoln.

![screenshot](images/boat-gate-test.png)

\--- /task \---