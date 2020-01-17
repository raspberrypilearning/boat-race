## Akadályok és erősítők

Jelenleg a játék **túl** könnyű, ezért hozzá fogsz adni új dolgokat, amelyektől érdekesebb lesz.

Először hozzáadsz néhány erősítést, amelyek felgyorsítják a hajót.

\--- task \---

Szerkeszd a játéktér hátterét, adj hozzá néhány fehér erősítő nyilat.

![képernyőkép](images/boat-boost.png)

\--- /task \---

\--- task \---

Most adj hozzá kódblokkokat a `mindig`{:class="block3control"} ciklushoz, hogy a hajó szereplő 3-mal több lépést tegyen, ha hozzáér egy fehér nyílhoz.

![boat-sprite](images/boat_resize.png)

```blocks3
ha <touching color [#FFFFFF] ?> akkor 
  menj (3) lépést
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
mindig
end

fordulj ↻ (1) fokot

⚑ -ra kattintáskor
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
⚑ -ra kattintáskor
mindig 
  fordulj ↻ (1) fokot
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---