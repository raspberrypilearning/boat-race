## Dodajanje časovnika

Zdaj boš igri dodal časovnik, tako da bo igralec moral priti na otok čim hitreje.

\--- task \---

Odru dodaj novo spremenljivko `čas`{: class = "block3variables"}.

![posnetek zaslona](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Svojemu časovniku lahko določiš tudi izgled, tako da spremeniš način, na katerega se spremenljivka prikazuje.

\--- /task \---

\--- task \---

Odru dodaj bloke kode, tako da bo časovnik prišteval čas, dokler čoln ne bo dosegel otoka.

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
spremeni [čas v] za (0.1)

ko kliknemo na zastavico

ponavljaj
konec

počakaj (0.1) sekund

nastavi [čas v] na [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
ko kliknemo na zastavico
nastavi [čas v] na [0]
ponavljaj
počakaj (0.1) sekund
spremeni [čas v] za (0.1)
konec
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---