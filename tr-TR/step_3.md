## Controlling the boat

Oyuncu fare ile tekne görüntüsünü kontrol eder.

\--- task \---

Tekneye, sol alt köşede başlayıp ardından fare imlecini takip edeceği kodu ekleyin.

![boat-sprite](images/boat_resize.png)

```blocks3
bayrak (0)
yönünde
noktaya tıkladığında x: (-190) y: (-150)
sonsuza kadar
noktaya (fare imleci v)
hareket ettirin (1)
```

\--- /task \---

\--- task \---

Yeşil bayrağa tıklayın ve fareyi hareket ettirerek **kodunuzu test edin**. Tekne sprite'ı fare imlecine doğru hareket ediyor mu?

![ekran görüntüsü](images/boat-mouse.png)

\--- no-print \---

![ekran görüntüsü](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![ekran görüntüsü](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

Tekne fare imlecine ulaşırsa ne olur? Dene ve sorunun ne olduğunu gör.

\--- /task \---

\--- task \---

To stop this from happening, you need to add an `if`{:class="block3control"} block to your code, so that the boat sprite only moves if it is more than 5 pixels away from the mouse pointer.

\--- hints \--- \--- hint \---

The boat should only point towards the mouse pointer and move `if`{:class="block3control"} the `distance to the mouse pointer`{:class="block3sensing"} is `greater than 5 pixels`{:class="block3operators"}.

\--- / ipucu - - ipucu -

Tekne görüntüsü için kodunuza eklemeniz gereken bloklar şunlardır:

![tekne-görüntüsü](images/boat_resize.png)

```blocks3
eğer < [] > [] > ardından

(mesafe (fare imleci v))
```

\--- / ipucu - - ipucu -

Kodunuz şöyle görünmelidir:

![tekne-görüntüsü](images/boat_resize.png)

```blocks3
bayrak (0)
yönünde
noktaya tıklandığında x: (-190) y: (-150)
sonsuza
eğer <((fare imleci v)) > [5]> sonra
nokta işaretçi v)
hareket (1) adım
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your code again to check whether the problem is now fixed.

\--- /task \---