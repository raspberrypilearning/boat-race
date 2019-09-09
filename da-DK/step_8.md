## Forhindringer og boostere

Lige nu er spillet **langt** for nemt, så du vil tilføje nogle ting for at gøre det mere interessant.

For det første vil du tilføje nogle boostere for at fremskynde båden.

\--- task \---

Rediger din scene baggrund ved at tilføje i nogle hvide booster pile.

![screenshots](images/boat-boost.png)

\--- /task \---

\--- task \---

Tilføj nu flere kodeblokke til din båds `evigt`{: class = "block3control"} løkke, så bådesprite bevæger tre ekstra trin, når den rører en hvid pil. ![båd-sprite](images/boat_resize.png)

```blocks3
hvis <touching color [#FFFFFF] ?> så
bevæger sig (3) trin
slutter
```

\--- /task \---

\--- task \---

Test dit spil for at se om dine nye boosterpile hurtigere bådene.

\--- /task \---

Dernæst tilføjer du en spinderport, som båden skal undgå.

\--- task \---

Tilføj et nyt sprite, der ligner dette, og kalder det 'gate':

![skærmbillede](images/boat-gate.png)

Sørg for, at portens sprite farve er den samme som træbarriens farve.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![Port](images/gate.png)

```blocks3
for evigt
ende

drej cw (1) grader

når flag klikkes
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

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