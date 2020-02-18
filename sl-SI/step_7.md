## Dodajanje časovnika

Zdaj boš igri dodal časovnik, tako da bo igralec moral priti na otok čim hitreje.

--- task ---

Odru dodaj novo spremenljivko `čas`{:class="block3variables"}.

![posnetek zaslona](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Svojemu časovniku lahko določiš tudi izgled, tako da spremeniš način, na katerega se spremenljivka prikazuje.

--- /task ---

--- task ---

Odru dodaj bloke kode, tako da bo časovnik prišteval čas, dokler čoln ne bo dosegel otoka.

--- hints --- --- hint ---

`Ko kliknemo na zastavico`{:class="block3control"} na odru, `nastavi čas na 0`{:class="block3variables"}. Znotraj `ponavljaj`{:class="block3control"} zanke, boš moral najprej `počakati 0,1 sekund`{:class="block3control"}, nato pa `spremeniti čas za 0,1`{:class="block3variables"}.

--- /hint --- --- hint ---

To so bloki kode, ki jih potrebuješ:

![oder](images/stage.png)

```blocks3
spremeni [čas v] za (0.1)

ko je kliknjena zelena zastavica

ponavljaj
konec

počakaj (0.1) sekund

nastavi [čas v] na [0]
```

--- /hint --- --- hint ---

Tvoja koda naj bi izgledala tako:

![oder](images/stage.png)

```blocks3
ko je kliknjena zelena zastavica
nastavi [čas v] na [0]
ponavljaj
počakaj (0.1) sekund
spremeni [čas v] za (0.1)
konec
```

--- /hint --- --- /hints ---

--- /task ---

--- task ---

Preizkusi igro, da vidiš, kako hitro lahko prideš s čolnom do otoka!

![posnetek zaslona](images/boat-variable-test.png)

--- /task ---