## Ovire in pospeševalci

Trenutno je igra **resnično** preveč enostavna, zato boš dodal še nekaj stvari, ki jo bodo naredile bolj zanimivo.

Najprej boš dodali nekaj pospeševalcev, ki bodo pohitrili čoln.

\--- task \---

Uredi ozadje odra, tako da dodaš nekaj belih puščic za pospeševanje.

![posnetek zaslona](images/boat-boost.png)

\--- /task \---

\--- task \---

Sedaj v zanko `ponavljaj`{: class = "block3control"} dodaj bloke kode, ki bodo figuro čolna premaknile za tri dodatne korake, kadar se čoln dotakne bele puščice.

![boat-sprite](images/boat_resize.png)

```blocks3
če <touching color [#FFFFFF] ?> potem
pojdi (3) korakov
konec
```

\--- /task \---

\--- task \---

Test your game to see whether your new booster arrows speed up the boat.

\--- /task \---

Next you'll add a spinning gate that the boat has to avoid.

\--- task \---

Add a new sprite that looks like this, and call it 'gate':

![screenshot](images/boat-gate.png)

Make sure that the colour of the gate sprite is the same as the colour of the wooden barriers.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \---

Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![gate](images/gate.png)

```blocks3
ponavljaj
konec

obrni se za (1) stopinj v desno

ko kliknemo na zastavico
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
ko kliknemo na zastavico
ponavljaj
obrni se za (1) stopinj v desno
konec
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---