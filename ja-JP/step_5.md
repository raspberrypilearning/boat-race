## 勝利！

\--- task \--- ここで別の`もし`{:class = "block3control"}ステートメントをボートスプライトのコードに追加します。これにより、プレーヤーがボートを黄色の島に到着させたときにプレイヤーが勝利するようになります。

ボートが無人島についたら、「やったー!」と言ってゲームが終了するようにします。

\--- hints \--- \--- hint \--- `ずっと` {:class = "block3control"}ループ内にコードブロックを追加して、、プレイヤーが勝利したかどうかをチェックし続けるようにします。

`もし`{:class="block3control"} ボートが島の色に`触れた`{:class="block3sensing"}ら、`'YEAH!'と秒間言って`{:class="block3looks"}、ゲームが終わるように`すべてを止める`{:class="block3control"}ようにします。 \--- / hint \--- \--- hint \--- 必要なコードブロックは次のとおりです。 ![ボートのスプライト](images/boat_resize.png)

```blocks3
[やった] と (2) 秒言う

もし <[#ffff99] 色に触れた> なら
end

stop [all v]

```

\--- / hint \--- \--- hint \--- コードは次のようになります： ![ボートのスプライト](images/boat_resize.png)

```blocks3
もし <[#ffff99] 色に触れた> なら 
  [やったー!] と (2) 秒言う
  stop [all v]
end
```

追加するコードは`ずっと`{:class="block3control"} ループの中にあることが必要であることを忘れないようにしてください。 \--- /hint \--- \--- /hints \--- \--- /task \---