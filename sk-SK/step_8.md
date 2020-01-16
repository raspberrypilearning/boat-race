## Prekážky a vylepšenia

Teraz je hra **príliš** ľahká, takže pridajme niekoľko vecí, aby sme ju spravili zaujímavejšou.

Najskôr pridaj zrýchľovače, ktoré zvýšia rýchlosť loďky.

\--- task \---

Uprav pozadie scény tak, že doň pridáš niekoľko bielych šípok, ktoré budú slúžiť ako zrýchľovače.

![snímka obrazovky](images/boat-boost.png)

\--- /task \---

\--- task \---

Do scenára loďky teraz pridaj bloky do cyklu `opakuj stále`{:class="block3control"} tak, aby sa loďka posunula o 3 kroky naviac, keď sa dotkne bielej šípky.

![boat-sprite](images/boat_resize.png)

```blocks3
ak <dotýkaš sa [#FFFFFF] ?> 
  dopredu (3)
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
opakuj stále
end

vpravo ↻ (1)

pri kliknutí na ⚑
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
pri kliknutí na ⚑
opakuj stále 
  vpravo ↻ (1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---