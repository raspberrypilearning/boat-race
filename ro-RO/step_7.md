## Adăugarea unui cronometru

Acum vei adăuga un cronometru la jocul tău pentru ca jucătorul să fie nevoit să ajungă cât mai repede la insulă.

\--- task \---

Adaugă o nouă variabilă numită `timp`{:class="block3variables"} pe Scena ta.

![captură de ecran](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

De asemenea, poți alege aspectul cronometrului tău schimbând modul în care este afișată noua ta variabilă.

\--- /task \---

\--- task \---

Acum, adaugă blocuri de cod pe Scena ta pentru ca cronometrul să numere până când barca ajunge la insulă.

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
modifică [timp v] cu (0.1)

când se dă click pe stegulețul verde

la infinit
end

așteaptă (0.1) secunde

setează [timp v] la [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
când se dă click pe stegulețul verde
setează [timp v] la [0]
la infinit
așteaptă (0.1) secunde
modifică [timp v] cu (0.1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---