## Engeller ve güçlendiriciler

Şu anda oyun **far** çok kolay, bu yüzden daha ilginç hale getirmek için bazı şeyler katacak.

İlk önce, tekneyi hızlandırmak için bazı güçlendiriciler ekleyeceksiniz.

\--- task \---

Bazı beyaz güçlendirici oklar ekleyerek Sahne Alanı düzeninizi düzenleyin.

![ekran görüntüsü](images/boat-boost.png)

\--- /task \---

\--- task \---

Şimdi teknenizin `sonsuza`koduna daha fazla kod bloğu ekleyin. {: Class = "block3control"} döngü.

![boat-sprite](images/boat_resize.png)

```blocks3
<touching color [#FFFFFF] ?> ise
hamle (3) adım
sonu
```

\--- /task \---

\--- task \---

Test your game to see whether your new booster arrows speed up the boat.

\--- /task \---

Next you'll add a spinning gate that the boat has to avoid.

\--- task \---

Add a new sprite that looks like this, and call it 'gate':

![screenshot](images/boat-gate.png)

Make sure that the colour of the gate sprite is the same as the colour of the wooden barriers.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \---

Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![gate](images/gate.png)

```blocks3
sonsuza kadar
son

bayrak tıklandığında cw (1) derece

döndür
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
bayrak
sonsuza dek
tıklatıldığında cw (1) derece
son
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---