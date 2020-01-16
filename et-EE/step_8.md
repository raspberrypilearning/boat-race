## Takistused ja võimendid

Praegu on mäng **kaugele** liiga lihtne, nii et lisate mõned asjad, mis muudavad selle huvitavamaks.

Esiteks lisate paadi kiirendamiseks mõned võimendid.

\--- ülesanne \---

Redigeerige oma lavastuse tausta, lisades mõnedele valged võimendnooled.

![ekraanipilt](images/boat-boost.png)

\--- / ülesanne \---

\--- ülesanne \---

Nüüd lisage oma paadi `forever`{: class = "block3control" silmusesse veel mitu koodiplokki nii, et paadi spriit liigub kolm ekraani, kui see puudutab valget noolt.

![boat-sprite](images/boat_resize.png)

```blocks3
kui <touching color [#FFFFFF] ?> siis
liiguta (3) samme

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
igavesti
lõpp

pöörake cw (1) kraadi

kui lipp klõpsati
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
kui lipp klõpsas
igavesti
pööret cw (1) kraadi
otsa
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---