## Sudaranje!

Trenutno, tvoj brod može ploviti kroz drvene prepreke. Popravimo to.

\--- task \---

Bit će ti potrebna dva kostima za brod: jedan normalni i jedan kada se brod sudari. Kloniraj kostim broda i jedan nazovi 'normalan', a drugi 'udaren'.

\--- /task \---

\--- task \---

Klikni na kostim 'udaren' i odaberi alat 'Označi'. Sada možeš uhvatiti komadiće broda, premještati ih i rotirati tako da brod izgleda kao da je razbijen.

![screenshot](images/boat-hit-costume.png)

\--- /task \---

\--- task \---

Dodaj naredbe brodu tako da se sudari i razbije kada dodirne smeđe drvene dijelove.

\--- hints \--- \--- hint \--- Dodaj naredbe unutar petlje `ponavljaj` kojima će se stalno provjeravati je li brod udario u prepreku. `Ako` brod `dodiruje` smeđu boju, `promijeni kostim u 'udaren'`, `reci Neeee! 2 sekunde` i onda `promijeni kostim u normalan`. Konačno, potrebno je`okreni se k strelica miša` i `idi na početnu poziciju`. \--- /hint \--- \--- hint \--- Trebat ćeš sljedeće naredbe: ![screenshot](images/boat-hit-blocks.png) \--- /hint \--- \--- hint \--- Tvoj kod treba izgledati ovako: ![screenshot](images/boat-hit-code.png) \--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also make sure that your boat always starts out looking 'normal'.

Ako sada pokušaš ploviti kroz drvenu prepreku, tvoj brod bi se trebao razbiti i vratiti na početnu poziciju.

![screenshot](images/boat-crash.png)

\--- /task \---