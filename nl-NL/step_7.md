## Een timer toevoegen

Laten we een timer aan je spel toevoegen, zodat de speler zo snel mogelijk naar het onbewoonde eiland moet.

\--- task \---

Maak een nieuwe variabele met de naam `tijd`{:class="block3variables"} aan.

![screenshot](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Je timer kan op verschillende manieren worden weergegeven.

\--- /task \---

\--- task \---

Voeg nu code toe, zodat de tijd oploopt tot de boot het onbewoonde eiland bereikt.

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
verander [tijd v] met (0.1)

wanneer op groene vlag wordt geklikt

herhaal
end

wacht (0.1) sec.

maak [tijd v] [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
wanneer op groene vlag geklikt
maak [tijd v] [0]
herhaal
wacht (0,1) sec.
verander [tijd v] met (0,1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---