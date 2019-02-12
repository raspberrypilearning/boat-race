## Zamanlayıcı eklemek

Artık oyununuza bir zamanlayıcı ekleyeceksiniz, böylece oyuncu adaya mümkün olduğu kadar çabuk ulaşmak zorunda.

\--- task \---

Sahne Alanı'na `kez`{: class = "block3variables"} adlı yeni bir değişken ekleyin.

![ekran görüntüsü](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Yeni değişkeninizin görüntülenme şeklini değiştirerek zamanlayıcınıza bir görünüm de seçebilirsiniz.

\--- /task \---

\--- task \---

Şimdi Sahne Alanı'na kod blokları ekleyin, böylece tekne adaya ulaşana kadar zamanlayıcı sayılır.

\--- tavsiyeleri \--- \--- ipucu \--- evre, üzerinde `yeşil bayrak tıklandığında`{: Sınıf = "block3control"}, `0 saati ayarlamak`{: Sınıf = "block3variables "}. İçinde senin `sonsuza`{: class = "block3control"} döngü, ilk gerekir `0.1 sn bekleyin`: sonra {class = "block3control"}, `0,1 ile değişim zamanı`{: class = "block3variables" }. \--- / hint \--- \--- hint \--- İhtiyacınız olan kod blokları: ![evre](images/stage.png)

```blocks3
(0.1) [zaman v] yerine

bayrak tıklandığında

sonsuza
uca

bekleme (0.1) saniye

set [zaman v] [0]
```

\--- / hint \--- \--- hint \--- Yeni kodunuzun şöyle görünmesi gerekenler: ![evre](images/stage.png)

```blocks3
bayrak
tıklandığında [zaman v] 'nin sonsuza kadar [0]
olmasını sağlayın
bekleyin (0.1) saniye
[zaman v]' ı (0.1)

```

\--- / ipucu \--- \--- / ipuçları \---

\--- /görev \---

\--- task \---

Oyununuzu test edin ve tekneyi adaya ne kadar hızlı götürebileceğinizi görün!

![ekran görüntüsü](images/boat-variable-test.png)

\--- /task \---