## Trk!

Trenutno lahko čoln pluje tudi skozi lesene ograje! To moraš zdaj popraviti.

--- task ---

Tvoja figura čolna potrebuje dva videza: en navaden videz in enega, ko čoln trešči ob oviro. Podvoji figuro tvojega čolna in poimenuj prvi videz "normalno", drugega pa "trk".

--- /task ---

--- task ---

Klikni na videz 'trk' in uporabit orodje **Izberi** da zgrabiš kose videza in jih premakneš in obračaš, da bo videti, kot da je čoln razpadel na koščke.

![posnetek zaslona](images/boat-hit-costume-annotated.png)

--- /task ---

--- task ---

Sedaj dodaj svojemu čolnu kodo, da se, kadar se dotakne rjave lesene ovire, zaleti in razpade,.

--- hints --- --- hint ---

Dodaj bloke kode znotraj zanke `ponavljaj`{:class="block3control"}, da bo tvoja koda še naprej preverjala, ali se je figura čolna zaletela. Če se je zaletela, mora koda ponastaviti položaj figure čolna.

`če`{:class="block3control"} se čoln `dotika`{:class="block3sensing"} rjave barve lesa, `zamenjaj videz na trk`{:class="block3looks"}, in reci `reči Neeeeee! za 2 sekundi`{:class="block3looks"}, nato pa `zamenjaj videz nazaj na normalno`{:class="block3looks"}. Nazadnje figuro `obrni navzgor`{:class="block3motion"} in `pojdi na začetno pozicijo`{:class="block3motion"}.

--- /hint --- --- hint ---

To so bloki kode, ki jih potrebuješ:

![figura čolna](images/boat_resize.png)

```blocks3
če <touching color [ ] ?> potem
konec

pojdi na X: (-190) y: (-150)

zamenjaj videz na (trk v)

obrni se v smer (0)

zamenjaj videz na (normalno V)

reci [Neeeeee!] za (2) sekund
```

--- /hint --- --- hint ---

Tvoja koda naj bi izgledala tako:

![figura čolna](images/boat_resize.png)

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

--- /hint --- --- /hints ---

--- /task ---

--- task ---

Dodaj tudi kodo, ki bo poskrbela, da bo tvoj čoln na začetku vedno videti 'normalno'.

Ponovno preizkusi svojo kodo. Če poskusiš zapeljati svoj čoln skozi leseno oviro, bi se sedaj moral zaleteti in premakniti nazaj na začetno pozicijo.

![posnetek zaslona](images/boat-crash.png)

--- /task ---