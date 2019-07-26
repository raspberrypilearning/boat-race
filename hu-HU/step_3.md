## A hajó irányítása

A játékos az egérrel irányítja a hajót.

\--- task \--- Adj kódot a hajó szereplőhöz úgy, hogy a bal alsó sarokból felfelé induljon, majd kövesse az egér mutatóját.

![hajó szereplő](images/boat_resize.png)

```blocks3
⚑ -ra kattintáskor
nézz (0) fokos irányba
ugorj ide: x: (-190) y: (-150)
mindig 
  nézz (egérmutató v) felé
  menj (1) lépést
end
```

\--- /task \---

\--- task \---

**Teszteld a kódod** a zöld zászlóra kattintva és az egeret mozgatva. Megy a hajó az egérmutató irányába?

![képernyőkép](images/boat-mouse.png)

\--- no-print \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- /no-print \---

\--- print-only \--- ![screenshot](images/boat-pointer-test-anim.png) \--- /print-only \---

\--- /task \---

\--- task \---

Mi történik, ha a hajó eléri az egérmutatót? Próbáld ki, hogy megtudd, mi a probléma.

\--- /task \---

\--- task \---

Ahhoz, hogy ez ne történhessen meg, hozzá kell adj egy `ha`{:class="block3control"} blokkot a kódodhoz, azért, hogy a hajó szereplő csak akkor mozogjon, ha több, mint 5 képpont távolságra van az egérmutatótól.

\--- hints \--- \--- hint \--- A hajónak csak akkor kell mutatnia az egérmutató felé, és csak akkor kell mennie, `ha`{:class="block3control"} az `egérmutató távolsága`{:class="block3sensing"} `nagyobb, mint 5 képpont`{:class="block3operators"}. \--- /hint \--- \--- hint \--- Ezek a kód blokkok, amelyeket hozzá kell adni a hajó szereplő kódjához: ![hajó szereplő](images/boat_resize.png)

```blocks3
ha <[ ] > [ ]> akkor

((egérmutató v) távolsága)
```

\--- /hint \--- \--- hint \--- Így kell kinéznie a kódodnak: ![hajó szereplő](images/boat_resize.png)

```blocks3
⚑ -ra kattintáskor
nézz (0) fokos irányba
ugorj ide: x: (-190) y: (-150)
mindig 
  ha <((egérmutató v) távolsága) > [5]> akkor 
    nézz (egérmutató v) felé
    menj (1) lépést
  end
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Teszteld újra a kódodat, hogy ellenőrizd, megoldottad-e a problémát.

\--- /task \---