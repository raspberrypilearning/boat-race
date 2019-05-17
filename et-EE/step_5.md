## Võitnud!

\--- ülesanne \--- Lisa veel `kui`{: class = "block3control"} oma paadi sprite koodile, nii et mängija võidab, kui paat saabub kollasesse saaresse.

Kui paat saarele jõuab, peaks mäng ütlema „YEAH!” Ja siis peaks see lõppema.

\--- hints \--- \--- vihje \--- Te peate lisama oma `igavesti`{: class = "block3control" silmusesse veel mitu koodiplokki, nii et teie kood kontrollib, kas mängija on võitnud:

`kui`{: class = "block3control"} paat on `puudutades`{: class = "block3sensing"} saare värvi, peate `ütlema "YEAH!" 2 sekundit`{: class = "block3looks"} ja seejärel `peatada kõik`{: class = "block3control"} mängu lõpetamiseks. \--- / vihje \--- \--- vihje \--- Siin on vajalikud koodiplokid: ![paadi-sprite](images/boat_resize.png)

```blocks3
ütle [YEAH!] (2) sekundit

kui <touching color [#FFFF99] ?> siis
lõppu

peatus [kõik v]

```

\--- / vihje \--- \--- vihje \--- Siin on, mida teie uus kood peaks välja nägema: ![paadi-sprite](images/boat_resize.png)

```blocks3
kui <touching color [#FFFF99] ?> siis
ütlevad [YEAH!] (2) sekundit
stop [all v]
lõpp
```

Ärge unustage, et see uus kood peab olema sees `forever`{: class = "block3control"} silmus. \--- / vihje \--- \--- / vihjed \--- \--- / ülesanne \---