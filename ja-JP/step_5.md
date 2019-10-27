## 勝利！

\--- task \--- ここで別の`もし`{:class = "block3control"}ステートメントをボートスプライトのコードに追加します。これにより、プレーヤーがボートを黄色の島に到着させたときにプレイヤーが勝利するようになります。

ボートが無人島についたら、「YEAH!」と言ってゲームが終了するようにします。

\--- hints \--- \--- hint \--- `ずっと` {:class = "block3control"}ループ内にコードブロックを追加して、、プレイヤーが勝利したかどうかをチェックし続けるようにします。

`もし`{:class="block3control"} ボートが島の色に`触れた`{:class="block3sensing"}ら、`'YEAH!'と秒間言って`{:class="block3looks"}、ゲームが終わるように`すべてを止める`{:class="block3control"}ようにします。 \--- / hint \--- \--- hint \--- 必要なコードブロックは次のとおりです。 ![boat-sprite](images/boat_resize.png)

```blocks3
say [YEAH!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
```

Don't forget that this new code needs to be inside the `forever`{:class="block3control"} loop. \--- /hint \--- \--- /hints \--- \--- /task \---