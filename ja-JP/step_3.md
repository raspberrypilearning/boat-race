## ボートを制御する

プレイヤーはマウスでボートのスプライトを制御します。

--- task ---

ボートのスプライトにコードを追加して、ボートのスプライトが左下隅で上向きで動き出し、マウスポインターを追いかけるようにします。

![ボートのスプライト](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
point towards (マウスのポインター v)
move (1) steps
```

--- /task ---

--- task ---

緑の旗をクリックしてからマウスを動かし、**コードをテストしましょう。**ボートのスプライトはマウスポインターに向かって移動しますか？

![スクリーンショット](images/boat-mouse.png)

--- no-print ---

![スクリーンショット](images/boat-pointer-test-anim.gif)

--- /no-print ---

--- print-only ---

![スクリーンショット](images/boat-pointer-test-anim.png)

--- /print-only ---

--- /task ---

--- task ---

ボートがマウスポインターに追いつくとどうなりますか？何が問題なのか確認してみましょう。

--- /task ---

--- task ---

そうならないように、`もし`{:class="block3control"} ブロックをコードに追加して、マウスポインターからの距離が5ピクセルより大きいときだけボートのスプライトを動かすようにしましょう。

--- hints ---
 --- hint ---

`もし`{:class="block3control"} `マウスポインターまでの距離`{:class="block3sensing"} が`5ピクセルより大きい`{:class="block3operators"} ときだけ、ボートがマウスポインターに向かって動くようにします。

--- /hint --- --- hint ---

こちらが、ボートスプライトのコードに追加する必要があるコードブロックです。

![ボートのスプライト](images/boat_resize.png)

```blocks3
if <[ ] > [ ]> then

(distance to (マウスのポインター v))
```

--- /hint --- --- hint ---

コードは次のようになります。

![ボートのスプライト](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
+if <(distance to (マウスのポインター v)) > [5]> then
point towards (マウスのポインター v)
move (1) steps
```

--- /hint ------ /hints ---

--- /task ---

--- task ---

コードをもう一度テストして、問題が修正されたかどうかを確認します。

--- /task ---