## Çarpışma!

Şu anda, tekne sprite ahşap engellerin üzerinden kolayca yelken açabilir! Bunu şimdi düzelteceksin.

\--- task \---

Tekne sprite için iki kostüm gerekir: biri normal kostüm, diğeri tekne çöktüğünde. Tekne sprite kostümünü çoğaltın ve bir kostüme 'normal' ve diğer 'isabet' adını verin.

\--- /task \---

\--- task \---

'Hit' kostümünüzü tıklayın ve kostümün parçalarını almak için **Select** aracını kullanın ve teknenin parçalara çarpmış gibi görünmesi için onları hareket ettirin ve döndürün.

![ekran görüntüsü](images/boat-hit-costume-annotated.png)

\--- /görev \---

\--- task \---

Şimdi teknenize kod ekleyin; böylelikle kahverengi ahşap bariyerlere dokunduğunda çarpar ve kırılır.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
eğer <touching color [ ] ?> sonra
son

, x: (-190) y: (-150)

geçiş kostümü (v) v yönünde

nokta (0)

geçiş kostümü (normal v)

deyin, (2 saniye
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
bayrak (0)
yönünde
noktaya tıklandığında x: (-190) y: (-150)
sonsuza
eğer <((fare imleci v)) > [5]> sonra
noktaya (fare- işaretçi v)
hareket (1) adım
ucu
ise <touching color [#663b00] ?> daha sonra
(v) 'vurmak için anahtar kostüm
demek [Noooooo!] (2) saniye için
(normal v) geçiş kostüm
yönünde alanına (0)
x'e git: (-190) y: (-150)
sonuç
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---