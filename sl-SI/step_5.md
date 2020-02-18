## Zmaga!

--- task ---

Dodaj še en `če`{:class="block3control"} pogoj v kodo figure čolna, tako da igralec zmaga, kadar se uspešno pripelje do rumenega otoka.

Ko bo čoln prispel do otoka, bi morala igra reči 'SUPERCA!', potem pa naj se konča.

--- hints --- --- hint ---

Dodatne bloke kode moraš vstaviti v zanko `ponavljaj`{:class="block3control"}, da bo tvoja koda redno preverjala ali je igralec zmagal:

`če`{:class="block3control"} se čoln `dotika`{:class="block3sensing"} barve otoka, `reci "SUPERCA! za 2 sekundi`{:class="block3looks"} in nato `ustavi vse`{:class="block3control"}, da končaš igro.

--- /hint --- --- hint ---

To so bloki kode, ki jih potrebuješ:

![figura čolna](images/boat_resize.png)

```blocks3
reci [SUPERCA!] za (2) sekund

če <se dotika barve [#FFFF99]?> potem
konec

ustavi [vse v]

```

--- /hint --- --- hint ---

Tvoja koda naj bi izgledala tako:

![figura čolna](images/boat_resize.png)

```blocks3
če <se dotika barve [#FFFF99]?> potem
reci [SUPERCA!] za (2) sekund
ustavi [vse v]
konec
```

Ne pozabi, da mora biti ta nova koda znotraj zanke `ponavljaj`{:class="block3control"}.

--- /hint --- --- /hints --- --- /task ---