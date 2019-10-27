## クラッシュ！

現時点では、ボートのスプライトは木製の壁を簡単に通過できます！これを修正していきましょう。

\--- task \---

ボートのコスチュームとして、普通のコスチュームとクラッシュしたときのコスチュームの２つが必要です。「boat」コスチュームを複製して一方を「normal」に、もう一方を「hit」という名前にしてください。

\--- /task \---

\--- task \---

「hit」コスチュームをクリックし、**選択**ツールでボートの一部を囲み、それらを移動させたり回転させたりして、ボートがクラッシュして粉々になったように見えるようにします。

![スクリーンショット](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

そしてボートにコードを追加して、茶色の木製の壁に触れるとクラッシュして壊れるようにしましょう。

\--- hints \--- \--- hint \--- `ずっと` {:class = "block3control"}ループ内にコードブロックを追加して、ボートスプライトがクラッシュしたかどうかをチェックし続け、クラッシュした場合、ボートスプライトの位置をリセットするようにします。

` もし ` {:class = "block3control"}ボートが木の茶色に`触れた` {:class = "block3sensing"}ら、`ヒットしたコスチュームに切り替え` {:class = "block3looks"}、 <0> Noooo！と2秒言い</code> {:class = "block3looks"}、その後`通常の衣装に戻ります` {:class = "block3looks"}。 最後に、ボートを`上向きにし` {:class = "block3motion"}、`開始位置に移動` {:class = "block3motion"}します。

\--- / hint \--- \--- hint \--- 必要なコードブロックは次のとおりです: ![boat-sprite](images/boat_resize.png)

```blocks3
もし<[茶] 色に触れた> なら
 コスチュームを(hit v) にする
 [Noooooo!] と (1) 秒言う
 コスチュームを(normal v) にする
 [0] 度に向ける
 x座標を(-190)、 y座標を(-150) にする
```

\--- / hint \--- \--- hint \--- コードは次のようになります： ![boat-sprite](images/boat_resize.png)

```blocks3
緑のフラグが押されたとき
(0) 度に向ける
x座標を(-190)、y座標を(-150) にする
ずっと
 もし<(マウスポインター v) までの距離>>(5)
 (マウスポインター v) へ向ける
 (1) 歩動かす
 おわり
 もし<[茶] 色に触れた> なら
 コスチュームを(hit v) にする
 [Noooooo!] と (1) 秒言う
 コスチュームを(normal v) にする
 [0] 度に向ける
 x座標を(-190)、 y座標を(-150) にする
 おわり
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![スクリーンショット](images/boat-crash.png)

\--- /task \---