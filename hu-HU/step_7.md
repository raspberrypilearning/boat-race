## Időzítő hozzáadása

Most hozzáadsz egy időzítőt a játékodhoz, így a játékosnak minél rövidebb idő alatt kell eljutnia a szigetre.

\--- task \---

Adj hozzá egy új változót a játéktérhez `idő`{:class="block3variables"} névvel.

![képernyőkép](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Kiválaszthatod az időzítő megjelenését, így különböző módokon jelenhet meg az új változód.

\--- /task \---

\--- task \---

Most adj hozzá kódblokkokat a játéktérhez, hogy az időzítő felfelé számoljon, amíg a hajó el nem éri a szigetet.

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
[idő v] változzon (0.1)

⚑ -ra kattintáskor

mindig
end

várj (0.1) mp-et

[idő v] legyen [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
⚑ -ra kattintáskor
[idő v] legyen [0]
mindig 
  várj (0.1) mp-et
  [idő v] változzon (0.1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---