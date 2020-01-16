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

\--- hints \--- \--- hint \--- Pe Scenă, `când se dă click pe stegulețul verde`{:class="block3control"}, `setează timp la 0`{:class="block3variables"}. În interiorul buclei `la infinit`{:class="block3control"}, va trebui mai întâi să `aștepți 0.1 secunde`{:class="block3control"}, iar apoi să `modifici timp cu 0.1`{:class="block3variables"}. \--- /hint \--- \--- hint \--- Iată blocurile de cod de care ai nevoie: ![scenă](images/stage.png)

```blocks3
modifică [timp v] cu (0.1)

când se dă click pe stegulețul verde

la infinit
end

așteaptă (0.1) secunde

setează [timp v] la [0]
```

\--- /hint \--- \--- hint \--- Așa ar trebui să arate codul: ![scenă](images/stage.png)

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

Teastează-ți jocul și vezi cât de repede poți ajunge la insulă!

![captură de ecran](images/boat-variable-test.png)

\--- /task \---