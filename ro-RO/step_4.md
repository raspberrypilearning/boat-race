## Accidentele!

În acest moment, barca poate naviga pur și simplu printre barierele de lemn! O sa repari asta acum.

\--- task \---

O să ai nevoie de două costume pentru barca ta: unul normal și unul pentru barca care se lovește de lemne. Dublează costumul bărcii și denumește unul dintre ele „normal” iar celălalt „lovită”.

\--- /task \---

\--- task \---

Dă click pe costumul „lovită” și folosește unealta **Selectează** pentru a prinde bucățile din costum și a le muta și roti pentru a face barca să pară că s-a făcut bucăți.

![captură de ecran](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Acum, adaugă codul la barca ta astfel încât să se lovească și rupă atunci când atinge bucățile maro de lemn.

\--- hints \--- \--- hint \--- Trebuie să adaugi blocuri de cod în bucla ta `la infinit`{:class="block3control"} astfel încât codul tău să verifice mereu dacă barca s-a lovit, iar dacă s-a lovit, codul trebuie să reseteze poziția bărcii.

`dacă`{:class="block3control"} barca `atinge`{:class="block3sensing"} culoarea maro a lemnului, trebuie să `schimbe costumul la lovită`{:class="block3looks"}, `spune Nuuuu! pentru 2 secunde`{:class="block3looks"}, iar apoi `schimbă costumul la normal`{:class="block3looks"}. În cele din urmă, va trebui să te `orientezi în sus`{:class="block3motion"} și să `mergi la poziția de start`{:class="block3motion"}.

\--- /hint \--- \--- hint \--- Iată blocurile de cod de care ai nevoie: ![barcă](images/boat_resize.png)

```blocks3
dacă <atinge culoarea []?> atunci
end

mergi la x: (-190) y: (-150)

schimbă costumul la (lovită v)

orientează-te în direcția (0)

schimbă costumul la (normal v)

spune [Nuuuu!] pentru (2) secunde
```

\--- /hint \--- \--- hint \--- Așa ar trebui să arate codul: ![barcă](images/boat_resize.png)

```blocks3
când se dă click pe stegulețul verde
orientează-te în direcția (0)
mergi la x: (-190) y: (-150)
la infinit
dacă <(distanța până la (cursorul mouse-ului v)) > [5]> atunci
orientează-te spre (cursorul mouse-ului v)
mergi (1) pași
end
dacă <atinge culoarea [#663b00]?> atunci
end
mergi la x: (-190) y: (-150)
schimbă costumul la (lovită v)
orientează-te în direcția (0)
schimbă costumul la (normal v)
spune [Nuuuu!] pentru (2) secunde
schimbă costumul la (normal v)
orientează-te în direcția (0)
mergi la x: (-190) y: (-150)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

De asemenea, trebuie să te asiguri că barca arată „normal” la începutul oricărei curse.

Testează-ți din nou codul. Dacă încerci să navighezi barca printr-o barieră din lemn, barca ar trebui să se lovească și apoi să se întoarcă înapoi la poziția sa de pornire.

![captură de ecran](images/boat-crash.png)

\--- /task \---