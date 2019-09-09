## Ovire in ojačevalci

Zdaj igra je **daleč** preveč enostavno, tako da bo dodal nekaj stvari, da bi bilo bolj zanimivo.

Najprej boste dodali nekaj ojačevalcev za pospešitev plovila.

\--- task \---

Uredite ozadje Stage, tako da dodate nekaj belih puščic.

![posnetek zaslona](images/boat-boost.png)

\--- /task \---

\--- task \---

Sedaj dodajte več kodnih blokov na zanko `vedno`{: class = "block3control"}, tako da bo žig ladje premaknil tri dodatne korake, ko se dotakne bele puščice. ![čoln](images/boat_resize.png)

```blocks3
če <touching color [#FFFFFF] ?> potem
premaknete (3) koraka
konec
```

\--- /task \---

\--- task \---

Preizkusite igro, da vidite, ali vaše nove pospeševalne puščice pospešijo čoln.

\--- /task \---

Nato boste dodali vrteča se vrata, ki jih mora čoln izogibati.

\--- task \---

Dodajte nov duh, ki izgleda takole, in ga pokličite »vrata«:

![posnetek zaslona](images/boat-gate.png)

Prepričajte se, da je barva vratnega duhu enaka barvi lesenih ovir.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![vrata](images/gate.png)

```blocks3
za vedno
konec

obrni cw (1) stopinj

ko je zastavica kliknila
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

```blocks3
ko je zastavica kliknila
vedno
obrni cw (1) stopinj
konec
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---