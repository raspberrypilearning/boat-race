## ボートを制御する

\--- task \---

Add this code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![ボートのスプライト](images/boat_resize.png)

```blocks3
⚑ が押されたとき
(0) 度に向ける
x座標を (-190) 、y座標を (-150) にする
ずっと 
(mouse-pointer v) へ向ける
(1) 歩動かす
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

Add code to the boat sprite so it only point towards the mouse pointer and moves `if`{:class="block3control"} the `distance to the mouse pointer`{:class="block3sensing"} is `greater than 5 pixels`{:class="block3operators"}.

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
+if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

\--- /task \---

\--- task \---

コードをもう一度テストして、問題が修正されたかどうかを確認します。

\--- /task \---