## Akadályok és erősítők

Jelenleg a játék **túl** könnyű, ezért hozzá fogsz adni új dolgokat, amelyektől érdekesebb lesz.

Először hozzáadsz néhány erősítést, amelyek felgyorsítják a hajót.

\--- task \---

Szerkeszd a játéktér hátterét, adj hozzá néhány fehér erősítő nyilat.

![képernyőkép](images/boat-boost.png)

\--- /task \---

\--- task \---

Most adj hozzá kódblokkokat a `mindig`{:class="block3control"} ciklushoz, hogy a hajó szereplő 3-mal több lépést tegyen, ha hozzáér egy fehér nyílhoz.

![hajó szereplő](images/boat_resize.png)

```blocks3
ha <touching color [#FFFFFF] ?> akkor 
  menj (3) lépést
end
```

\--- /task \---

\--- task \---

Teszteld a játékodat, nézd meg, hogy az erősítő nyilak fegyorsítják-e a hajót.

\--- /task \---

Most hozzáadsz egy forgó kaput, amelyet a hajónak el kell kerülnie.

\--- task \---

Adj hozzá egy új szereplőt, amely így néz ki, és nevezd "kapu"-nak:

![képernyőkép](images/boat-gate.png)

Győződj meg róla, hogy a kapu szereplő színe megegyezik a fa akadályok színével.

![képernyőkép](images/brown-hsv.png)

\--- /task \---

\--- task \---

Győződj meg róla, hogy a kapu szereplő középpontja középen helyezkedik el.

![képernyőkép](images/boat-center.png)

\--- /task \---

\--- task \---

Adj hozzá kódot a kapu szereplőhöz, hogy mindig lassan forogjon.

\--- hints \--- \--- hint \---

Adj hozzá kódblokkokat a szereplőhöz, hogy `forduljon 1 fokot`{:class="block3motion"} `mindig`{:class="block3control"}.

\--- /hint \--- \--- hint \---

Íme a szükséges kódblokkok:

![kapu](images/gate.png)

```blocks3
mindig
end

fordulj ↻ (1) fokot

⚑ -ra kattintáskor
```

\--- /hint \--- \--- hint \---

A kódnak így kell kinéznie:

![kapu](images/gate.png)

```blocks3
⚑ -ra kattintáskor
mindig 
  fordulj ↻ (1) fokot
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Teszteld újra a játékodat. Most ott kell lennie a forgó kapunak, amelyet a hajónak el kell kerülnie.

![képernyőkép](images/boat-gate-test.png)

\--- /task \---