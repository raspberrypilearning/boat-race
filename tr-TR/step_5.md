## Kazanan!

\--- görev \--- Şimdi başka eklemek `eğer`onlar tekne sarı adaya varmak yaparken oyuncu kazanır böylece tekne birleşik resmin koduna açıklama: {class = "block3control"}.

Tekne adaya ulaştığında oyun 'YEAH!' Demeli ve sonra bitmeli.

\--- ipuçları \--- \--- ipucu \--- İçinde fazla kod blokları eklemek gerekir senin `sonsuza`{: class = "block3control"} döngü kodunuzu oyuncu kazandı olmadığını kontrol eder, böylece:

``{: class = "block3control"} tekne `dokunuyorsa`{: class = "block3sensing"} adanın rengini, `'YEAH!' 2 saniye boyunca`{: class = "block3looks"} ve daha sonra `oyunu bitirmek için`{: class = "block3control"} 'i durdurur. \--- / hint \--- \--- hint \--- İhtiyacınız olan kod blokları: ![tekne-sprite](images/boat_resize.png)

```blocks3
[YEAH!] deyin (2) saniye

ise <touching color [#FFFF99] ?> sonra
son

durur [tümü v]

```

\--- / hint \--- \--- hint \--- Yeni kodunuzun şöyle görünmesi gerekenler: ![tekne-sprite](images/boat_resize.png)

```blocks3
eğer <touching color [#FFFF99] ?> ise
(2) saniye boyunca [YEAH!] diyorsa
durdur [tümü v]
son
```

Bu yeni kodun sonsuza dek `olması gerektiğini unutmayın`{: class = "block3control"} döngü. \--- / ipucu \--- \--- / ipuçları \--- \--- / görev \---