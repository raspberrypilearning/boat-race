## Zamanlayıcı eklemek

Artık oyununuza bir zamanlayıcı ekleyeceksiniz ve böylelikle oyuncu adaya mümkün olduğu kadar çabuk ulaşmak zorunda kalacak.

\--- task \---

Sahnenize `zaman`{: class = "block3variables"} adlı yeni bir değişken ekleyin.

![ekran görüntüsü](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Yeni değişkeninizin görüntülenme şeklini değiştirerek zamanlayıcınıza bir görünüm de seçebilirsiniz.

\--- /task \---

\--- task \---

Şimdi Sahnenize kod blokları ekleyin ve böylece tekne adaya ulaşana kadar geçen süreyi zamanlayıcı saysın.

\--- hints \--- \--- hint \---

Sahnede, `yeşil bayrak tıklandığında`{:class="block3control"}, `zamanı 0 olarak ayarla` {:class="block3variables"}. </code>Sonsuz</code>{:class="block3control"} döngünüzün içinde, öncelikle `0.1 saniye bekleyin`{:class="block3control"} ve ardından `zamanı 0.1 olarak değiştirin</0>{:class="block3variables"}.</p>

<p>--- /hint ---
--- hint ---</p>

<p>İhtiyacınız olan kod blokları:</p>

<p><img src="images/stage.png" alt="aşama" /></p>

<pre><code class="blocks3">değiştir [zaman v] şu şekilde (0.1)

bayrak tıklandığında

daima
bitir

bekle (0.1) saniye

ayarla [zaman v] şu şekilde [0]
`</pre> 

\--- /hint \--- \--- hint \---

Yeni kodunuz şöyle görünmelidir:

![aşama](images/stage.png)

```blocks3
bayrak tıklandığında
ayarla [zaman v] şu şekilde [0]
daima
bekle (0.1) saniye
değiştir [zaman v] şu şekilde (0.1)
bitir
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Oyununuzu test edin ve tekneyi adaya ne kadar çabuk götürebileceğinizi görün!

![ekran görüntüsü](images/boat-variable-test.png)

\--- /task \---