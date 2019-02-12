## A hajó irányítása

A játékos az egérrel vezérli a hajót.

\--- task \--- Kód hozzáadása a hajó sprite-hez, hogy a bal alsó sarokban felfelé induljon, majd követi az egérmutatót.

![csónak-sprite](images/boat_resize.png)

```blocks3
ha a zászló
pontra kattintott (0)
megy x: (-190) y: (-150)
örökre
pont felé (egérmutató v)
lépés (1) lépés
```

\--- / feladat \---

\--- feladat \---

**Ellenőrizze a kódját** a zöld zászlóra kattintva és az egér mozgatásával. A hajó ugrik az egérmutató felé?

![screenshot](images/boat-mouse.png)

\--- no-print \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- / nincs nyomtatás \---

\--- csak nyomtatás \--- ![screenshot](images/boat-pointer-test-anim.png) \--- csak nyomtatás \---

\--- / feladat \---

\--- feladat \---

Mi történik, ha a hajó eléri az egérmutatót? Próbálja ki, hogy mi a probléma.

\--- / feladat \---

\--- feladat \---

Ennek megakadályozásához meg kell adnia egy `if`{: class = "block3control"} blokkot a kódjához, hogy a hajó sprite csak akkor mozog, ha több mint 5 pixel van az egérmutatótól.

\--- tippeket \--- \--- csipetnyi \--- A csónak csak felé mutasson az egér mutatót, és mozgassa `, ha`{: class = „block3control”} a `távolságot az egér mutatót`{: class = "block3sensing"} `nagyobb, mint 5 pixel`{: class = "block3operators"}. \--- / tipp \--- \--- tipp \--- Ezek a kódblokkok, amelyeket hozzá kell adni a hajó sprite kódjához: ![csónak-sprite](images/boat_resize.png)

```blocks3
ha < [] > [] > majd

(távolság az egérmutatóhoz v)
```

\--- / tipp \--- \--- tipp \--- Ez az, amit a kódodnak kell kinéznie: ![csónak-sprite](images/boat_resize.png)

```blocks3
ha a zászló
pontra kattintva (0)
megy x: (-190) y: (-150)
örökre
ha <(távolság (egérmutató v) > [5]> majd
pont felé (egér- v)
lépés (1) lépés
```

\--- / tipp \--- \--- / hints \---

\--- / feladat \---

\--- feladat \---

Ellenőrizze újra a kódot, hogy ellenőrizze, hogy a probléma már rögzítve van.

\--- / feladat \---