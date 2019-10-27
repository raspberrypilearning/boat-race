## ボートの制御

プレイヤーはマウスでボートのスプライトを制御します。

\--- task \--- 左下隅で上向きに動き出し、マウスポインターをたどるように、ボートスプライトにコードを追加します。

![boat-sprite](images/boat_resize.png)

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

\--- no-print \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- /no-print \---

\--- print-only \--- ![screenshot](images/boat-pointer-test-anim.png) \--- /print-only \---

\--- /task \---

\--- task \---

ボートがマウスポインターに到達するとどうなりますか？問題が何であるかを確認してください。

\--- /task \---

\--- task \---

そうならないように、コードに`もし…なら`{:class="block3control"} のブロックを入れて、ボートがマウスから5ピクセル以上離れている時だけ動くようにしましょう。

\--- hints \--- \--- hint \--- ボートは`もし`{:class="block3control"} 、`マウスポインターまでの距離`{:class="block3sensing"} が`が5ピクセルより大きい`{:class="block3operators"} 時だけ、マウスポインターの方に移動しなければなりません \--- / hint \--- \--- hint \--- これらは、ボートスプライトのコードに追加する必要があるコードブロックです。 ![boat-sprite](images/boat_resize.png)

```blocks3
もし < [] > [] > ならば

((マウスポインター v) までの距離)
```

\--- / hint \--- \--- hint \--- コードは次のようになります： ![boat-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your code again to check whether the problem is now fixed.

\--- /task \---