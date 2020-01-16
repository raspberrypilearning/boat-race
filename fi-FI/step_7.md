## Ajastimen lisääminen

Lisätään peliin ajastin, joten pelaajan on päästävä saarelle niin pian kuin mahdollista.

\--- task \---

Lisää uusi muuttuja nimeltä `aika`{:class="block3variables"} Esiintymislavallesi.

![kuvakaappaus](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Voit myös valita ajastimen ulkoasun muuttamalla uuden muuttujan näyttötapaa.

\--- /task \---

\--- task \---

Lisää koodilohkoja esiintymislavallesi niin, että aika kasvaa, kunnes vene saapuu saarelle.

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
lisää muuttujaan [aika v] arvo (0.1)

kun klikataan ⚑

ikuisesti
end

odota (0.1) sekuntia

aseta [aika v] arvoon [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
kun klikataan ⚑
aseta [aika v] arvoon [0]
ikuisesti 
  odota (0.1) sekuntia
  lisää muuttujaan [aika v] arvo (0.1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---