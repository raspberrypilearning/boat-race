## Accidentele!

Pentru moment, barca ta poate naviga printre barajele de lemne! Haide sa rezolvăm asta.

\--- task \---

O sa ai nevoie de doua profiluri pentru barca ta, unul normal, si unul pentru barca care se loveste de lemne. Dubleaza profilul barcii, si pune-i un nume ca 'normal' iar celalalt 'lovitura'.

\--- /task \---

\--- task \---

Apasa pe profil 'lovitura' si alege instrumentul Selectare, pentru a apuca aschii din barca pentru a le misca si roti astfel incat sa para ca un accident.

![captură de ecran](images/boat-hit-costume.png)

\--- /task \---

\--- task \---

Acum adauga codul la barca ta astfel incat sa se loveasca si rupa atunci cand atinge bucati de lemn.

\--- hints \--- \--- hint \--- Adauga codul tau `mereu` in bucla repetitiva, astfel incat, acesta sa verifice mereu, daca barca se loveste. `dacă`barca`atinge`culoarea lemnului, va trebui să`o schimbi în profilul barcă lovită`, `say Nuuuuu! pentru 2 secunde`, si apoi `schimba inapoi pe profilul`. La final, vei trebui sa mergi`sus` si `la pozitia de start`. \--- /hint \--- \--- hint \--- Acestea sunt blocurile de comenzi necesare: ![screenshot](images/boat-hit-blocks.png) \--- /hint \--- \--- hint \--- Asa ar trebui sa arate: ![screenshot](images/boat-hit-code.png) \--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

De asemenea trebuie sa te asiguri ca barca, la inceputul cursei, are activat profilul 'normal'.

Acum daca vei incerca sa navigi peste un banc de lemne, ar trebui sa vezi cum se loveste barca si cum se intoarce la pozitia de start.

![captură de ecran](images/boat-crash.png)

\--- /task \---