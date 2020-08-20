## Çarpışma!

Şu anda, tekne sprite ahşap engellerin üzerinden kolayca yelken açabilir! Bunu şimdi düzelteceksin.

--- task ---

Tekne görüntüsü için iki kostüm gerekir: biri normal kostüm, diğeri tekne çöktüğünde. Tekne görüntüsü kostümünü çoğaltın ve bir kostüme 'normal' ve diğer 'isabet' adını verin.

--- /task ---

--- task ---

'Hit' kostümünüzü tıklayın ve kostümün parçalarını almak için **Select** aracını kullanın ve teknenin parçalara çarpmış gibi görünmesi için onları hareket ettirin ve döndürün.

![ekran görüntüsü](images/boat-hit-costume-annotated.png)

--- /task ---

--- task ---

Şimdi teknenize kod ekleyin; böylelikle kahverengi ahşap bariyerlere dokunduğunda çarpar ve kırılır.

--- hints ---
 --- hint ---

`Sonsuz`{:class="block3control"} döngünüzün içine kod blokları eklemeniz gerekiyor, böylece kodunuz tekne kuklasının çarpışıp çarpışmadığını kontrol eder ve çarpışmışsa da kodun tekne kuklasının konumunu sıfırlamasını sağlar.

`Eğer`{:class="block3control"} tekne, odunun kahvrengi rengine `değiyorsa`{:class="block3sensing"}, `kostümüne geçmeli`, `2 saniyeliğine Hayıııır! demeli`{:class="block3looks"} ve ardından `normal kostüme geri dömelisiniz`{:class="block3looks"}. Son olarak, `işaret etmeli`{:class="block3motion"} ve `başlangıç pozisyonuna geri`{:class="block3motion"} dönmelisiniz.

--- /hint --- --- hint ---

İhtiyacınız olan kod blokları:

![tekne-görüntüsü](images/boat_resize.png)

```blocks3
if <touching color [ ] ?> then
end

go to x: (-190) y: (-150)

switch costume to (darbe almış v)

point in direction (0)

switch costume to (normal v)

say [Hayırrrr!] for (2) seconds
```

--- /hint --- --- hint ---

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
say [Hayırrrr!] for (2) seconds
switch costume to (normal v)
point in direction (0)
go to x: (-190) y: (-150)
end
```

--- /hint ------ /hints ---

--- /task ---

--- task ---

Ayrıca, teknenizin görüntüsünün her zaman 'normal' olarak görünmeye başladığından emin olmak için kod eklemelisiniz.

Kodunuzu tekrar test edin. Tekneyi şu anda tahta bir bariyerden geçirmeye çalışırsanız, tekne çarpmalı ve ardından başlangıç pozisyonuna geri dönmelidir.

![ekran görüntüsü](images/boat-crash.png)

--- /task ---