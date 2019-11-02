## タイマーを追加する

次に、ゲームにタイマーを追加して、プレーヤーができるだけ早く島に着かなければならないようにしましょう。

\--- task \---

` time` {:class = "block3variables"}という新しい変数をステージに追加します。

![スクリーンショット](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

新しい変数の表示方法を変更して、タイマーの外観を選択することもできます。

\--- /task \---

\--- task \---

ボートが島に到着するまでタイマーがカウントアップするように、ステージにコードブロックを追加します。

\--- hints \--- \--- hint \--- On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}. \--- /hint \--- \--- hint \--- Here are the code blocks you'll need: ![stage](images/stage.png)

```blocks3
change [time v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [time v] to [0]
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![stage](images/stage.png)

```blocks3
when flag clicked
set [time v] to [0]
forever
wait (0.1) seconds
change [time v] by (0.1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![スクリーンショット](images/boat-variable-test.png)

\--- /task \---