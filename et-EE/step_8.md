## Takistused ja võimendid

Praegu on mäng **kaugele** liiga lihtne, nii et lisate mõned asjad, mis muudavad selle huvitavamaks.

Esiteks lisate paadi kiirendamiseks mõned võimendid.

\--- ülesanne \---

Redigeerige oma lavastuse tausta, lisades mõnedele valged võimendnooled.

![ekraanipilt](images/boat-boost.png)

\--- / ülesanne \---

\--- ülesanne \---

Nüüd lisage oma paadi `forever`{: class = "block3control" silmusesse veel mitu koodiplokki nii, et paadi spriit liigub kolm ekraani, kui see puudutab valget noolt. ![paadi-sprite](images/boat_resize.png)

```blocks3
kui <touching color [#FFFFFF] ?> siis
liiguta (3) samme

```

\--- / ülesanne \---

\--- ülesanne \---

Testi oma mängu, et näha, kas teie uus võimendi nool kiirendab paati.

\--- / ülesanne \---

Järgmisena lisate ketruse värava, mida paat peab vältima.

\--- ülesanne \---

Lisage uus ilme, mis näeb välja selline ja nimetage seda "väravaks":

![ekraanipilt](images/boat-gate.png)

Veenduge, et värava sprite värv on sama mis puidust tõkete värv.

\--- / ülesanne \---

\--- ülesanne \---

Veenduge, et värava sprite keskpunkt paikneb keskel.

![ekraanipilt](images/boat-center.png)

\--- / ülesanne \---

\--- ülesanne \---

Lisage oma väravale kood, et muuta see aeglaselt spin.

\--- hints \--- \--- vihje \--- Lisa koodiplokid väravale, nii et see `muutub 1 kraadi`{: class = "block3motion"} `igavesti`{: class = "block3control"} . \--- / vihje \--- \--- vihje \--- Siin on vajalikud koodiplokid: ![värav](images/gate.png)

```blocks3
igavesti
lõpp

pöörake cw (1) kraadi

kui lipp klõpsati
```

\--- / vihje \--- \--- vihje \--- Siin on, mida teie uus kood peaks välja nägema: ![värav](images/gate.png)

```blocks3
kui lipp klõpsas
igavesti
pööret cw (1) kraadi
otsa
```

\--- / vihje \--- \--- / vihjed \---

\--- / ülesanne \---

\--- ülesanne \---

Testi oma mängu uuesti. Nüüd peaks teil olema ketrusvärav, mida peate oma paadi ümber segama.

![ekraanipilt](images/boat-gate-test.png)

\--- / ülesanne \---