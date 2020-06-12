## Çarpışma!

Şu anda, tekne sprite ahşap engellerin üzerinden kolayca yelken açabilir! Bunu şimdi düzelteceksin.

\--- task \---

Tekne görüntüsü için iki kostüm gerekir: biri normal kostüm, diğeri tekne çöktüğünde. Tekne görüntüsü kostümünü çoğaltın ve bir kostüme 'normal' ve diğer 'isabet' adını verin.

\--- /task \---

\--- task \---

'Hit' kostümünüzü tıklayın ve kostümün parçalarını almak için **Select** aracını kullanın ve teknenin parçalara çarpmış gibi görünmesi için onları hareket ettirin ve döndürün.

![ekran görüntüsü](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Şimdi teknenize kod ekleyin; böylelikle kahverengi ahşap bariyerlere dokunduğunda çarpar ve kırılır.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

İhtiyacınız olan kod blokları:

![tekne-görüntüsü](images/boat_resize.png)

```blocks3
if <touching color [ ] ?> then
end

go to x: (-190) y: (-150)

switch costume to (hit v)

point in direction (0)

switch costume to (normal v)

say [Noooooo!] for (2) seconds
```

\--- /hint \--- \--- hint \---

Kodunuz şöyle görünmelidir:

![tekne-görüntüsü](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
end
if <touching color [#663b00] ?> then
switch costume to (hit v)
say [Noooooo!] for (2) seconds
switch costume to (normal v)
point in direction (0)
go to x: (-190) y: (-150)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Ayrıca, teknenizin görüntüsünün her zaman 'normal' olarak görünmeye başladığından emin olmak için kod eklemelisiniz.

Kodunuzu tekrar test edin. Tekneyi şu anda tahta bir bariyerden geçirmeye çalışırsanız, tekne çarpmalı ve ardından başlangıç pozisyonuna geri dönmelidir.

![ekran görüntüsü](images/boat-crash.png)

\--- /task \---