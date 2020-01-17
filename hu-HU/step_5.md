## Győzelem!

\--- task \---

Most adj hozzá egy újabb `ha`{:class="block3control"} utasítást a hajó szereplőd kódjához, hogy a játékos nyerjen, ha sikerül elvezetnie a hajót a sárga szigetre.

Amikor a hajó eljut a szigetre, a játéknak azt kell mondania, hogy "IGEN!", aztán be kell fejeződnie.

\--- hints \--- \--- hint \---

További kódblokkokat kell hozzáadnod a `mindig`{: class = "block3control"} ciklushoz úgy, hogy a kódod folyamatosan ellenőrizze, hogy a játékos nyert-e:

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the colour of the island, you need to `say 'YEAH!' for 2 seconds`{:class="block3looks"} and then `stop all`{:class="block3control"} to end the game.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
mondd: [IGEN!] (2) másodpercig

ha <touching color [#FFFF99] ?> akkor
end

álljon le [minden feladat v]

```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
ha <touching color [#FFFF99] ?> akkor 
  mondd: [IGEN!] (2) másodpercig
  álljon le [minden feladat v]
end
```

Don't forget that this new code needs to be inside the `forever`{:class="block3control"} loop.

\--- /hint \--- \--- /hints \--- \--- /task \---