## Trk!

Trenutno lahko čoln pluje tudi skozi lesene ograje! To moraš zdaj popraviti.

\--- task \---

Tvoja figura čolna potrebuje dva videza: en navaden videz in enega, ko čoln trešči ob oviro. Podvoji figuro tvojega čolna in poimenuj prvi videz "normalno", drugega pa "trk".

\--- /task \---

\--- task \---

Klikni na videz 'trk' in uporabit orodje **Izberi** da zgrabiš kose videza in jih premakneš in obračaš, da bo videti, kot da je čoln razpadel na koščke.

![posnetek zaslona](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Sedaj dodaj svojemu čolnu kodo, da se, kadar se dotakne rjave lesene ovire, zaleti in razpade,.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
če <touching color [ ] ?> potem
konec

pojdi na X: (-190) y: (-150)

zamenjaj videz na (trk v)

obrni se v smer (0)

zamenjaj videz na (normalno V)

reci [Neeeeee!] za (2) sekund
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
ko kliknemo na zastavico
obrni se v smer (0)
pojdi na x: (-190) y: (-150)
ponavljaj
če <(razdalja do (kazalca miške v)) > [5]> potem
obrni se proti (kazalcu miške v)
pojdi (1) korakov
konec
če če <se dotika barve [#663B00]?> potem
zamenjaj videz na (trk v)
zamenjaj videz na (normalno V)
obrni se v smer (0)
pojdi na X: (-190) y: (-150)
reci [Neeeeee!] za (2) sekund
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---