## Hindernisse und Power-Ups

Also, dieses Spiel ist **echt** zu einfach, damit es interessanter wird, lass' uns einige Sachen ergänzen.

Fügen wir zuerst einige Beschleunigungen in dein Spiel ein, um das Boot schneller zu machen.

\--- task \---

Bearbeite dein Bühnenhintergrund und füge einige weiße Beschleunigungspfeile hinzu.

![Screenshot](images/boat-boost.png)

\--- /task \---

\--- task \---

Jetzt erweitere den Code in der `Wiederhole-fortlaufend`-Schleife des Bootes{:class="block3control"}, sodass es sich drei Schritte zusätzlich nach vorne bewegt, wenn es einen weißen Pfeil berührt.

![boat-sprite](images/boat_resize.png)

```blocks3
wenn <touching color [#FFFFFF] ?> dann 
gehe (3) er Schritt
ende
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
wiederhole fortlaufend
ende

drehe dich im Uhrzeigersinn um (1) Grad

Wenn die grüne Flagge angeklickt wird
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
Wenn grüne Flagge angeklickt wird
wiederhole fortlaufend
drehe dich im Uhrzeigersinn um (1) Grad
ende
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---