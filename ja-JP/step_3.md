## ボートを制御する

プレイヤーはマウスでボートのスプライトを制御します。

\--- task \---

ボートのスプライトにコードを追加して、ボートのスプライトが左下隅で上向きで動き出し、マウスポインターを追いかけるようにします。

![ボートのスプライト](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
point towards (mouse-pointer v)
move (1) steps
```

\--- /task \---

\--- task \---

緑の旗をクリックしてからマウスを動かし、**コードをテストしましょう。**ボートのスプライトはマウスポインターに向かって移動しますか？

![スクリーンショット](images/boat-mouse.png)

\--- no-print \---

![スクリーンショット](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![スクリーンショット](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

ボートがマウスポインターに追いつくとどうなりますか？何が問題なのか確認してみましょう。

\--- /task \---

\--- task \---

To stop this from happening, you need to add an `if`{:class="block3control"} block to your code, so that the boat sprite only moves if it is more than 5 pixels away from the mouse pointer.

\--- hints \--- \--- hint \---

`もし`{:class="block3control"} `マウスポインターまでの距離`{:class="block3sensing"} が`5ピクセルより大きい`{:class="block3operators"} ときだけ、ボートがマウスポインターに向かって動くようにします。

\--- /hint \--- \--- hint \---

These are the code blocks you need to add to the code for the boat sprite:

![ボートのスプライト](images/boat_resize.png)

```blocks3
もし <[ ] > [ ]> なら

((mouse-pointer v) までの距離)
```

\--- /hint \--- \--- hint \---

コードは次のようになります。

![ボートのスプライト](images/boat_resize.png)

```blocks3
⚑ が押されたとき
(0) 度に向ける
x座標を (-190) 、y座標を (-150) にする
ずっと 
もし <((mouse-pointer v) までの距離) > [5]> なら 
(mouse-pointer v) へ向ける
(1) 歩動かす
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

コードをもう一度テストして、問題が修正されたかどうかを確認します。

\--- /task \---