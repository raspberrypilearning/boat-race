## Taimeri lisamine

Nüüd lisate oma mängule taimerit, nii et mängija peab saare juurde minema nii kiiresti kui võimalik.

\--- ülesanne \---

Lisage oma etappi uus muutuja nimega `aeg`{: class = "block3variables"}.

![ekraanipilt](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Samuti saate valida oma taimerile oma uue muutuja kuvamise viisi.

\--- / ülesanne \---

\--- ülesanne \---

Nüüd lisage oma lava koodiplokid nii, et taimer loeb kuni paat jõuab saare.

\--- hints \--- \--- vihje \--- Etapis `kui klõpsatakse rohelist lippu`{: class = "block3control"}, `seadke aeg 0`{: class = "block3variables "}. Sisse oma `igavesti`{: class = "block3control"} loop, peate kõigepealt `ootama 0,1 sekundit`{: class = "block3control"}, seejärel `muutke aega 0,1`{: class = "block3variables" }. \--- / vihje \--- \--- vihje \--- Siin on vajalikud koodiplokid: ![etapis](images/stage.png)

```blocks3
muutke [aeg v] (0,1)

kui lipp klõpsas

igavesti
lõpp

oota (0,1) sekundit

set [aeg v] kuni [0]
```

\--- / vihje \--- \--- vihje \--- Siin on, mida teie uus kood peaks välja nägema: ![etapis](images/stage.png)

```blocks3
kui lipp klõpsas
set [time v] kuni [0]
igavesti
oodake (0,1) sekundit
muutus [aeg v] (0,1)
lõpp
```

\--- / vihje \--- \--- / vihjed \---

\--- / ülesanne \---

\--- ülesanne \---

Testi oma mängu ja vaata, kui kiiresti sa saad paati saarele!

![ekraanipilt](images/boat-variable-test.png)

\--- / ülesanne \---