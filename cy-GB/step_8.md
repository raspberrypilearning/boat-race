## Rhwystrau a chyflymu'r cwch

Mae’r gêm yma **llawer** rhy hawdd - awn ati i ychwanegu pethau i’w wneud yn fwy diddorol.

Yn gyntaf, fe wnawn ni ychwanegu ‘hwb’ i dy gêm, fydd yn cyflymu’r cwch.

\--- task \---

Golyga cefndir dy lwyfan ac ychwanega arwyddion gwyn.

![sgrinlun](images/boat-boost.png)

\--- /task \---

\--- task \---

Fe alli di nawr ychwanegu côd i’r ddolen `am byth`{:class="block3control"}, fel ei fod yn symud 3 cam ychwanegol pan mae’n cyffwrdd arwydd gwyn.

![boat-sprite](images/boat_resize.png)

```blocks3
os <cyffwrdd lliw [#FFFFFF] ?> yna 
  symud (3) cam
end
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
am byth
end

troi (1) gradd i'r dde

pan fo'r flag werdd yn cael ei glicio
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
pan fo'r flag werdd yn cael ei glicio
am byth 
  troi (1) gradd i'r dde
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---