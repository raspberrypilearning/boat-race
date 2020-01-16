## Preteky na čas

Teraz pridáš do hry stopky, takže hráč sa bude snažiť dostať na ostrov čo najrýchlejšie.

\--- task \---

Do scenára pridaj novú premennú a nazvi ju `čas`{:class="block3variables"}.

![snímka obrazovky](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Zmenou spôsobu zobrazenia premennej na scéne si môžeš zvoliť, aký budú mať stopky vzhľad.

\--- /task \---

\--- task \---

Teraz pridaj do scenára bloky tak, aby sa stopky spustili, keď loďka odštartuje a zastavili, keď loďka pripláva ku ostrovu.

\--- hints \--- \--- hint \---

Na scéne, `pri kliknutí na zelenú vlajku`{:class="block3control"}, `nastav čas na 0`{:class="block3variables"}. Vo vnútri cyklu `opakuj stále`{:class="block3control"}, najskôr `čakaj 0.1 sekundy`{:class="block3control"}, potom ` zmeň čas o 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Tu sú bloky, ktoré budeš potrebovať do scenára:

![scéna](images/stage.png)

```blocks3
zmeň [čas v] o (0.1)

pri kliknutí na ⚑

opakuj stále
end

čakaj (0.1) s

nastav [čas v] na [0]
```

\--- /hint \--- \--- hint \---

Takto by mal vyzerať tvoj scenár:

![scéna](images/stage.png)

```blocks3
pri kliknutí na ⚑
nastav [čas v] na [0]
opakuj stále 
  čakaj (0.1) s
  zmeň [čas v] o (0.1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Vyskúšaj si hru a zisti, ako rýchlo sa vieš dostať s loďkou na ostrov!

![snímka obrazovky](images/boat-variable-test.png)

\--- /task \---