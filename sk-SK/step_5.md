## Víťazstvo!

\--- task \---

Teraz do scenára pre loďku pridaj ďalší blok `ak`{:class="block3control"}, tak aby hráč vyhral hru, keď pripláva s loďkou až ku žltému ostrovu.

Keď loďka pripláva ku žltému ostrovu hra by mala ukázať bublinu 'HURÁ!' a potom by mala skončiť.

\--- hints \--- \--- hint \---

Potrebuješ pridať bloky do vnútra cyklu `opakuj stále`{:class="block3control"}, aby scenár neustále kontroloval či hráč vyhral hru:

`ak`{:class="block3control"} sa loďkou `dotýkaš`{:class="block3sensing"} ostrova žltej farby, ukáž `bublinu 'HURÁ!' na 2 sekundy`{:class="block3looks"} a potom `zastav všetko`{:class="block3control"} čím ukončíš hru.

\--- /hint \--- \--- hint \---

Tu sú bloky, ktoré budeš potrebovať do scenára:

![postava loďky](images/boat_resize.png)

```blocks3
bublina [HURÁ!] (2) s

ak <dotýkaš sa [#FFFF99] ?>
end

zastav [všetko v]

```

\--- /hint \--- \--- hint \---

Takto by mal vyzerať tvoj scenár:

![postava loďky](images/boat_resize.png)

```blocks3
ak <dotýkaš sa [#FFFF99] ?> 
  bublina [HURÁ!] (2) s
  zastav [všetko v]
end
```

Nezabudni, že táto nová časť scenára sa musí nachádzať vo vnútri cyklu `opakuj stále`{:class="block3control"}.

\--- /hint \--- \--- /hints \--- \--- /task \---