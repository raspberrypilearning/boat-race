## Forhindringer og boostere

Lige nu er spillet **langt** for nemt, så du vil tilføje nogle ting for at gøre det mere interessant.

For det første vil du tilføje nogle boostere for at fremskynde båden.

\--- task \---

Rediger din scene baggrund ved at tilføje i nogle hvide booster pile.

![screenshots](images/boat-boost.png)

\--- /task \---

\--- task \---

Tilføj nu flere kodeblokke til din båds `evigt`{: class = "block3control"} løkke, så bådesprite bevæger tre ekstra trin, når den rører en hvid pil.

![boat-sprite](images/boat_resize.png)

```blocks3
hvis <touching color [#FFFFFF] ?> så
bevæger sig (3) trin
slutter
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
for evigt
ende

drej cw (1) grader

når flag klikkes
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
når flag klikker
evigt
drej cw (1) grader
ende
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---