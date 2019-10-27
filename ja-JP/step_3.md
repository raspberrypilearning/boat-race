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

\--- hints \--- \--- hint \--- The boat should only point towards the mouse pointer and move `if`{:class="block3control"} the `distance to the mouse pointer`{:class="block3sensing"} is `greater than 5 pixels`{:class="block3operators"}. \--- /hint \--- \--- hint \--- These are the code blocks you need to add to the code for the boat sprite: ![boat-sprite](images/boat_resize.png)

```blocks3
if < [ ] > [ ] > then

(distance to (mouse-pointer v))
```

\--- /hint \--- \--- hint \--- This is what your code should look like: ![boat-sprite](images/boat_resize.png)

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