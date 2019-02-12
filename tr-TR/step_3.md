## Tekneyi kontrol etme

Oyuncu fare ile tekne sprite kontrol eder.

\--- görev \--- Botun hareketli yerine kod ekleyerek sol alt köşeden yukarı bakacak ve fare işaretçisini izleyecektir.

![tekne-sprite](images/boat_resize.png)

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

**Yeşil bayrağa tıklayarak ve fareyi hareket ettirerek kodunuzu** test edin. Tekne sprite fare işaretçisine doğru hareket ediyor mu?

![ekran görüntüsü](images/boat-mouse.png)

\--- baskı yok \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- / baskı yok \---

\--- sadece baskı \--- ![screenshot](images/boat-pointer-test-anim.png) \--- / sadece baskı \---

\--- /task \---

\--- task \---

Tekne fare imlecine ulaştığında ne olur? Sorunun ne olduğunu görmek için deneyin.

\--- /görev \---

\--- task \---

Bunun olmasını engellemek için, eğer kodunuza</code>{: class = "block3control"} bloğu varsa `eklemeniz gerekir, böylece tekne sprite sadece fare işaretçisinden 5 pikselden daha uzaktaysa hareket eder.</p>

<p>--- tavsiyeleri ---
--- ipucu ---
tekne fare işaretçisi doğru yönelir ve hareket sadece gerektiği <code>ise`{: Sınıf = "block3control"} `fare işaretçisi uzaklık`{: sınıf = "block3sensing"} `, 5 pikselden büyük`{: class = "block3operators"}. \--- / hint \--- \--- hint \--- Bunlar tekne sprite koduna eklemeniz gereken kod blokları: ![tekne-sprite](images/boat_resize.png)

```blocks3
eğer < [] > [] > ardından

(mesafe (fare imleci v))
```

\--- / ipucu \--- \--- ipucu \--- Kodunuzun şöyle görünmesi gereken şey: ![tekne-sprite](images/boat_resize.png)

```blocks3
bayrak (0)
yönünde
noktaya tıklandığında x: (-190) y: (-150)
sonsuza
eğer <((fare imleci v)) > [5]> sonra
nokta işaretçi v)
hareket (1) adım
```

\--- / ipucu \--- \--- / ipuçları \---

\--- /task \---

\--- task \---

Sorunun şimdi çözülüp çözülmediğini kontrol etmek için kodunuzu tekrar test edin.

\--- /task \---