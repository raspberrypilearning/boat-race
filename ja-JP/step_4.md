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

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \--- Here are the code blocks you need: ![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [ ] ?> then
end

go to x: (-190) y: (-150)

switch costume to (hit v)

point in direction (0)

switch costume to (normal v)

say [Noooooo!] for (2) seconds
```

\--- /hint \--- \--- hint \--- Here's what your code should look like: ![boat-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
end
if <touching color [#663b00] ?> then
switch costume to (hit v)
say [Noooooo!] for (2) seconds
switch costume to (normal v)
point in direction (0)
go to x: (-190) y: (-150)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![スクリーンショット](images/boat-crash.png)

\--- /task \---