## ぶつかった！

現時点では、ボートのスプライトは木製の壁を簡単に通過できます！これを修正していきましょう。

\--- task \---

ボートのコスチュームとして、通常のコスチュームと衝突したときのコスチュームの２つが必要です。「boat」コスチュームを複製して一方を「通常」に、もう一方を「衝突」という名前にしてください。

\--- /task \---

\--- task \---

「衝突」コスチュームをクリックし、**選択**ツールでボートの一部を囲み、それらを移動させたり回転させたりして、ボートがクラッシュして粉々になったように見えるようにします。

![スクリーンショット](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

そしてボートにコードを追加して、茶色の木製の壁に触れるとクラッシュして壊れるようにしましょう。

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
もし <touching color [ ] ?> なら
end

x座標を (-190) 、y座標を (-150) にする

コスチュームを (衝突t v) にする

(0) 度に向ける

コスチュームを (通常 v) にする

[うわーーー！] と (2) 秒言う
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
⚑ が押されたとき
(0) 度に向ける
x座標を (-190) 、y座標を (-150) にする
ずっと 
  もし <((mouse-pointer v) までの距離) > [5]> なら 
    (mouse-pointer v) へ向ける
    (1) 歩動かす
  end
  もし <touching color [#663b00] ?> なら 
    コスチュームを (衝突 v) にする
    [Noooooo!] と (2) 秒言う
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---