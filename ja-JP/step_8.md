## 障害物とブースター

今のままではゲームは**とても**簡単すぎるので、いろいろつけ足してもっとおもしろくしましょう。

最初に、ボートをスピードアップするためのブースターを追加します。

\--- task \---

白いブースター矢印を追加して、ステージの背景を編集します。

![スクリーンショット](images/boat-boost.png)

\--- /task \---

\--- task \---

ボートの`ずっと` {：class = "block3control"}ループにさらにコードブロックを追加して、ボートのスプライトが白い矢印に触れたときに、もう3歩動くようにします。

![boat-sprite](images/boat_resize.png)

```blocks3
もし <[#FFFFFF] 色に触れた> なら 
  (3) 歩動かす
end
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
ずっと
end

↻ (1) 度回す

⚑ が押されたとき
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
⚑ が押されたとき
ずっと 
  ↻ (1) 度回す
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---