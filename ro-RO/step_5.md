## Câștigă!

\--- task \--- Acum, adaugă altă instrucțiune `dacă`{:class="block3control"} la codul bărcii tale pentru ca jucătorul să câștige când acesta ajunge cu barca pe insula galbenă.

Atunci când barca ajunge la insulă, jocul ar trebui să spună „Bravoo!” și să se oprească.

\--- hints \--- \--- hint \--- Va trebui să mai adaugi blocuri de tip `la infinit`{:class="block3control"} pentru ca programul să verifice mereu dacă jucătorul a câștigat:

`dacă`{:class="block3control"} barca `atinge`{:class="block3sensing"} culoarea insulei, trebuie să `spui „Bravoo!” pentru 2 secunde`{:class="block3looks"} iar apoi să dai `stop totul`{:class="block3control"} pentru a încheia jocul. \--- /hint \--- \--- hint \--- Iată blocurile de cod de care ai nevoie: ![barcă](images/boat_resize.png)

```blocks3
spune [Bravoo!] pentru (2) secunde

dacă <atinge culoarea [#FFFF99]?> atunci
end

stop [totul v]

```

\--- /hint \--- \--- hint \--- Așa ar trebui să arate codul: ![barcă](images/boat_resize.png)

```blocks3
dacă <atinge culoarea [#FFFF99]?> atunci
spune [Bravoo!] pentru (2) secunde
stop [totul v]
end
```

Nu uita că acest cod nou trebuie să fie în interiorul buclei `la infinit`{:class="block3control"}. \--- /hint \--- \--- /hints \--- \--- /task \---