## Engeller ve güçlendiriciler

Şu anda oyun **far** çok kolay, bu yüzden daha ilginç hale getirmek için bazı şeyler katacak.

İlk önce, tekneyi hızlandırmak için bazı güçlendiriciler ekleyeceksiniz.

\--- task \---

Bazı beyaz güçlendirici oklar ekleyerek Sahne Alanı düzeninizi düzenleyin.

![ekran görüntüsü](images/boat-boost.png)

\--- /task \---

\--- task \---

Şimdi teknenizin `sonsuza`koduna daha fazla kod bloğu ekleyin. {: Class = "block3control"} döngü. ![tekne-sprite](images/boat_resize.png)

```blocks3
<touching color [#FFFFFF] ?> ise
hamle (3) adım
sonu
```

\--- /task \---

\--- task \---

Yeni yükseltici okların tekneyi hızlandırıp hızlandırmadığını görmek için oyununuzu test edin.

\--- /task \---

Sonra, teknenin kaçınması gereken bir dönüş kapısı ekleyeceksiniz.

\--- task \---

Buna benzeyen yeni bir sprite ekleyin ve buna 'kapı' diyor

![ekran görüntüsü](images/boat-gate.png)

Geçit sprite renginin ahşap bariyerlerin rengiyle aynı olduğundan emin olun.

\--- /task \---

\--- task \---

Gate sprite merkezinin ortasına yerleştirildiğinden emin olun.

![ekran görüntüsü](images/boat-center.png)

\--- /task \---

\--- task \---

Sonsuza dek yavaş yavaş dönmesini sağlamak için geçit sprite kodunu ekleyin.

\--- tavsiyeleri \--- \--- ipucu \--- bu şekilde kapı grafiğine kod blokları ekleyin `1 derece döner`{: Sınıf = "block3motion"} `sonsuza`{: Sınıf = "block3control"} . \--- / hint \--- \--- hint \--- İhtiyacınız olan kod blokları: ![kapı](images/gate.png)

```blocks3
sonsuza kadar
son

bayrak tıklandığında cw (1) derece

döndür
```

\--- / hint \--- \--- hint \--- Yeni kodunuzun şöyle görünmesi gerekenler: ![kapı](images/gate.png)

```blocks3
bayrak
sonsuza dek
tıklatıldığında cw (1) derece
son
```

\--- / ipucu \--- \--- / ipuçları \---

\--- /task \---

\--- task \---

Oyununuzu tekrar test edin. Şimdi teknenizi karıştırmak için gereken bir döndürme kapısına sahip olmalısınız.

![ekran görüntüsü](images/boat-gate-test.png)

\--- /task \---