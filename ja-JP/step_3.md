## ボートの制御

プレイヤーはマウスでボートのスプライトを制御します。

\--- task \--- 左下隅で上向きに動き出し、マウスポインターをたどるように、ボートスプライトにコードを追加します。

![ボートのスプライト](images/boat_resize.png)

```blocks3
⚑ が押されたとき
(0) 度に向ける
x座標を (-190) 、y座標を (-150) にする
ずっと 
  (mouse-pointer v) へ向ける
  (1) 歩動かす
end
```

\--- /task \---

\--- task \---

緑の旗をクリックしてからマウスを動かし、**コードをテストしましょう。**ボートのスプライトはマウスポインターに向かって移動しますか？

![スクリーンショット](images/boat-mouse.png)

\--- no-print \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- /no-print \---

\--- print-only \--- ![screenshot](images/boat-pointer-test-anim.png) \--- /print-only \---

\--- /task \---

\--- task \---

ボートがマウスポインターに到達するとどうなりますか？問題が何であるかを確認してください。

\--- /task \---

\--- task \---

そうならないように、コードに`もし…なら`{:class="block3control"} のブロックを入れて、ボートがマウスから5ピクセル以上離れている時だけ動くようにしましょう。

\--- hints \--- \--- hint \--- ボートは`もし`{:class="block3control"} 、`マウスポインターまでの距離`{:class="block3sensing"} が`が5ピクセルより大きい`{:class="block3operators"} 時だけ、マウスポインターの方に移動しなければなりません \--- / hint \--- \--- hint \--- これらは、ボートスプライトのコードに追加する必要があるコードブロックです。 ![ボートのスプライト](images/boat_resize.png)

```blocks3
もし <[ ] > [ ]> なら
end

((mouse-pointer v) までの距離)
```

\--- / hint \--- \--- hint \--- コードは次のようになります： ![ボートのスプライト](images/boat_resize.png)

```blocks3
⚑ が押されたとき
(0) 度に向ける
x座標を (-190) 、y座標を (-150) にする
ずっと 
  もし <((mouse-pointer v) までの距離) > [5]> なら 
    (mouse-pointer v) へ向ける
    (1) 歩動かす
  end
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

コードをもう一度テストして、問題が修正されたかどうかを確認します。

\--- /task \---