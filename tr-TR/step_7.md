## Zamanlayıcı eklemek

Artık oyununuza bir zamanlayıcı ekleyeceksiniz ve böylelikle oyuncu adaya mümkün olduğu kadar çabuk ulaşmak zorunda kalacak.

--- task ---

Sahnenize `zaman`{:class="block3variables"} adlı yeni bir değişken ekleyin.

![ekran görüntüsü](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Yeni değişkeninizin görüntülenme şeklini değiştirerek zamanlayıcınıza bir görünüm de seçebilirsiniz.

--- /task ---

--- task ---

Şimdi Sahnenize kod blokları ekleyin ve böylece tekne adaya ulaşana kadar geçen süreyi zamanlayıcı saysın.

--- hints ---
 --- hint ---

Sahnede, `yeşil bayrak tıklandığında`{:class="block3control"}, `zamanı 0 olarak ayarla`{:class="block3variables"}. `Sonsuz`{:class="block3control"} döngünüzün içinde, öncelikle `0.1 saniye bekleyin`{:class="block3control"} ve ardından `zamanı 0.1 olarak değiştirin`{:class="block3variables"}.

--- /hint ---
--- hint ---

İhtiyacınız olan kod blokları:

![aşama](images/stage.png)


```blocks3
change [zaman v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [zaman v] to [0]
```

--- /hint --- --- hint ---

Yeni kodunuz şöyle görünmelidir:

![aşama](images/stage.png)

```blocks3
when flag clicked
set [zaman v] to [0]
forever
wait (0.1) seconds
change [zaman v] by (0.1)
end
```

--- /hint ------ /hints ---

--- /task ---

--- task ---

Oyununuzu test edin ve tekneyi adaya ne kadar çabuk götürebileceğinizi görün!

![ekran görüntüsü](images/boat-variable-test.png)

--- /task ---