## Accidentele!

Pentru moment, barca ta poate naviga printre barajele de lemne! Haide sa o corectam.

\--- proba\---

O sa ai nevoie de doua profiluri pentru barca ta, unul normal, si unul pentru barca care se loveste de lemne. Dubleaza profilul barcii, si pune-i un nume ca 'normal' iar celalalt 'lovitura'.

\--- /proba\---

\--- proba\---

Apasa pe profil 'lovitura' si alege instrumentul Selectare, pentru a apuca aschii din barca pentru a le misca si roti astfel incat sa para ca un accident.

![screenshot](images/boat-hit-costume.png)

\--- /proba\---

\--- proba\---

Acum adauga codul la barca ta astfel incat sa se loveasca si rupa atunci cand atinge bucati de lemn.

\--- hints \--- \--- hint \--- Adauga codul tau `totdeauna` in bucla repetitiva, astfel incat, acesta sa verifice mereu, daca barca se loveste. `If` the boat is `touching` the brown colour of the wood, you need to `switch to the hit costume`, `say Noooo! pentru 2 secunde`, si apoi `schimba inapoi pe profilul`. La final, vei trebui sa mergi`sus` si `la pozitia de start`. \--- /hint \--- \--- hint \--- Acestea sunt blocurile de comenzi necesare: ![screenshot](images/boat-hit-blocks.png) \--- /hint \--- \--- hint \--- Asa ar trebui sa arate: ![screenshot](images/boat-hit-code.png) \--- /hint \--- \--- /hints \---

\--- /proba\---

\--- proba\---

You should also make sure that your boat always starts out looking 'normal'.

If you try to sail through a wooden barrier now, you should see that your boat crashes and moves back to the start.

![screenshot](images/boat-crash.png)

\--- /task \---