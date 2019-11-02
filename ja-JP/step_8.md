## 障害物とブースター

今のままではゲームは**とても**簡単すぎるので、いろいろつけ足してもっとおもしろくしましょう。

最初に、ボートをスピードアップするためのブースターを追加します。

\--- task \---

白いブースター矢印を追加して、ステージの背景を編集します。

![screenshot](images/boat-boost.png)

\--- /task \---

\--- task \---

ボートの`ずっと` {：class = "block3control"}ループにさらにコードブロックを追加して、ボートのスプライトが白い矢印に触れたときに、もう3歩動くようにします。 ![boat-sprite](images/boat_resize.png)

```blocks3
もし <[#FFFFFF] 色に触れた> なら 
  (3) 歩動かす
end
```

\--- /task \---

\--- task \---

ゲームをテストして、新しいブースター矢印がボートを加速するかどうかを確認します。

\--- /task \---

次に、ボートが避けなければならない回転ゲートを追加します。

\--- task \---

次のような新しいスプライトを追加し、「ゲート」という名前を付けます。

![スクリーンショット](images/boat-gate.png)

ゲートスプライトの色が木の障壁の色と同じであることを確認してください。

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

ゲートスプライトの中心が中央に配置されていることを確認します。

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

ゲートスプライトにコードを追加して、ゆっくりとずっと回転するようにします。

\--- hints \--- \--- hint \--- ゲートスプライトにコードブロックを追加して、ゲートが `ずっと`{:class="block3control"}`1度回る`{:class="block3motion"}.ようにします。 \--- /hint \--- \--- hint \--- 必要なコードブロックは次のとおりです。 ![gate](images/gate.png)

```blocks3
forever
end

turn cw (1) degrees

when flag clicked
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

```blocks3
when flag clicked
forever
turn cw (1) degrees
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---