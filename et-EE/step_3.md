## Paadi juhtimine

Mängija kontrollib paadi sprite hiirega.

\--- ülesanne - Lisage paadi paadile kood nii, et see algab vasakpoolses nurgas ülespoole ja järgneb hiirekursorile.

![paadi-sprite](images/boat_resize.png)

```blocks3
kui lipp klõpsas
punkti suunas (0)
minge x: (-190) y: (-150)
igavesti
punkti (hiirekursor v)
liiguta (1) sammu suunas
```

\--- / ülesanne \---

\--- ülesanne \---

**Testi oma koodi** klõpsates roheline lipp ja hiirt liigutades. Kas paat liigub hiirekursori suunas?

![ekraanipilt](images/boat-mouse.png)

\--- no-print \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- / ei-print \---

\--- ainult printimiseks \--- ![screenshot](images/boat-pointer-test-anim.png) \--- / ainult printimiseks \---

\--- / ülesanne \---

\--- ülesanne \---

Mis juhtub, kui paat jõuab hiirekursorini? Proovige seda, et näha, mis probleem on.

\--- / ülesanne \---

\--- ülesanne \---

Selle peatamiseks peate oma koodile lisama `kui`{: class = "block3control"}, nii et paadi sprite liigub ainult siis, kui see on rohkem kui 5 pikslit hiirekursorist eemal.

\--- hints \--- \--- vihje \--- Paat peaks suunama hiirekursori poole ja liikuma `kui`{: class = "block3control"} `kaugust hiirekursorist`{: class = "block3sensing"} on `suurem kui 5 pikslit`{: class = "block3operators"}. \--- / vihje \--- \--- vihje \--- Need on koodiplokid, mida peate paadi sprite koodile lisama: ![paadi-sprite](images/boat_resize.png)

```blocks3
kui < [] > [] > siis

(kaugus (hiirekursor v))
```

\--- / vihje \--- \--- vihje \--- See, mida teie kood peaks välja nägema: ![paadi-sprite](images/boat_resize.png)

```blocks3
kui lipp klõpsas
punkti suunas (0)
minge x: (-190) y: (-150)
igavesti
kui <(kaugus (hiirekursor v)) > [5]> siis
punkti (hiir- pointer v)
liiguta (1) samme
```

\--- / vihje \--- \--- / vihjed \---

\--- / ülesanne \---

\--- ülesanne \---

Kontrollige oma koodi uuesti, et kontrollida, kas probleem on nüüd fikseeritud.

\--- / ülesanne \---