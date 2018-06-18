## Upravljanje brodom

\--- task \---

Brodom ćeš upravljati pomoću miša. Dodaj naredbe svom brodu tako da krene iz donjeg lijevog kuta okrenut prema gore i slijedi pokazivač miša. **Testiraj svoj kod** kako bi se uvjerio da radi ono što bi trebao.

\--- hints \--- \--- hint \--- Kad je `kliknuta zelena zastavica`, tvoj brod treba `otići na početnu poziciju` i `okrenuti se prema gore`. Zatim treba `biti okrenut prema pokazivaču miša` i `pomaknuti se za 1 korak`. Ovo treba ponavljati `zauvijek`.

\--- /hint \--- \--- hint \--- Trebat ćeš ove blokove naredbi: ![screenshot](images/boat-move-blocks.png) \--- /hint \--- \--- hint \--- Tvoj kod treba izgledati ovako: ![screenshot](images/boat-move-code.png) \--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Klikom na zastavicu i pomicanjem miša testiraj svoj brod. Plovi li brod prema pokazivaču miša?

![screenshot](images/boat-mouse.png)

![screenshot](images/boat-pointer-test-anim.gif)

## \--- collapse \---

title: Ako imaš problema...

## image: images/image.png

**Napomena:** U Scratchu je trenutno pogreška i tvoj brod se možda neće pomicati prema pokazivaču miša. Ako se ovo dogodi, klikni strelicu u bloku `okreni se prema naprijed` i ponovno odaberi `pokazivač miša`.

![screenshot](images/boat-bug.png) \--- /collapse \---

\--- /task \---

\--- task \---

Što će se dogoditi ako brod dođe do strelice miša? Isprobaj.

\--- /task \---

\--- task \---

Da bi se to izbjeglo, potrebno je programu dodati naredbu `ako... onda` tako da se brod pomiče samo ako je od strelice miša udaljen više od 5 piksela.

\--- hints \--- \--- hint \--- Brod se treba okrenuti prema strelici miša i pomicati `ako` je `udaljenost do strelice miša` `veća od 5 piksela`. \--- /hint \--- \--- hint \--- Dodaj sljedeće naredbe brodu: ![screenshot](images/boat-pointer-blocks.png) \--- /hint \--- \--- hint \--- Tvoj kod treba izgledati ovako: ![screenshot](images/boat-pointer-code.png) \--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Ponovno isprobaj svoj brod i provjeri je li problem riješen.

\--- /task \---