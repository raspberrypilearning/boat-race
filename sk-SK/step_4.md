## Náraz!

V tejto chvíli dokáže loďka jednoducho preplávať cez drevené prekážky! Teraz to napravíš.

\--- task \---

Potrebuješ dva kostýmy pre loďku: jeden normálny a druhý, keď loďka narazí. Duplikuj kostým loďky a pomenuj jeden kostým ako 'normál' a druhý ako 'náraz'.

\--- /task \---

\--- task \---

Klikni na kostým 'náraz' a použi nástroj **Označ** na vybratie a uchopenie kúskov kostýmu. Uchopené kúsky kostýmu presuň a otoč tak, aby loďka vyzerala po náraze ako by sa rozbila na kusy.

![snímka obrazovky](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Teraz pridaj ku loďke scenár, ktorý spôsobí to, že loďka po dotyku s drevenými prekážkami narazí a rozpadne sa.

\--- hints \--- \--- hint \---

Potrebuješ pridať bloky do vnútra cyklu `opakuj stále`{:class="block3control"}, aby scenár neustále kontroloval či došlo k nárazu loďky. Po náraze musí scenár nastaviť loďku na štartovaciu pozíciu.

`ak`{:class="block3control"} sa loďkou `dotýkaš`{:class="block3sensing"} drevenej prekážky hnedej farby `zmeň kostým na náraz`{:class="block3looks"}, a ukáž `bublinu Nieeeeee! na 2 sekundy`{:class="block3looks"}, potom `zmeň kostým na normál`{:class="block3looks"}. Nakoniec sa otoč `smerom hore`{:class="block3motion"} a `skoč na štartovaciu pozíciu`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
ak <dotýkaš sa [ ] ?>
end

skoč na x: (-190) y: (-150)

zmeň kostým na (náraz v)

smerom (0)

zmeň kostým na (normál v)

bublina [Nieeeeee!] (2) s
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
pri kliknutí na ⚑
smerom (0)
skoč na x: (-190) y: (-150)
opakuj stále 
  ak <(vzdialenosť k (myš v)) > [5]> 
    smerom k (myš v)
    dopredu (1)
  end
  ak <dotýkaš sa [#663b00] ?> 
    zmeň kostým na (náraz v)
    bublina [Nieeeeee!] (2) s
    zmeň kostým na (normál v)
    smerom (0)
    skoč na x: (-190) y: (-150)
  end
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---