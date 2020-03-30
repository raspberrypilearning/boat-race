## 勝利！

--- task ---

ここで別の`もし`{:class="block3control"}ステートメントをボートスプライトのコードに追加します。これにより、プレーヤーがボートを黄色の島に到着させたときにプレイヤーが勝利するようになります。

ボートが無人島についたら、「やったー！」と言ってゲームが終了するようにします。

--- hints ---
 --- hint ---

`ずっと`{:class="block3control"}ループ内にコードブロックを追加して、プレイヤーが勝利したかどうかをチェックし続けるようにします。

`もし`{:class="block3control"} ボートが島の色に`触れた`{:class="block3sensing"}ら、`「やったー！］と2秒間言って`{:class="block3looks"}、ゲームを終了するために`すべてを止めます`{:class="block3control"}。

--- /hint --- --- hint ---

必要なコードブロックは次のとおりです。

![ボートのスプライト](images/boat_resize.png)

```blocks3
[やったー！] と (2) 秒言う

もし <touching color [#FFFF99] ?> なら
end

stop [すべてをとめる v]

```

--- /hint --- --- hint ---

コードは次のようになります。

![ボートのスプライト](images/boat_resize.png)

```blocks3
もし <touching color [#FFFF99] ?> なら 
[やったー！] と (2) 秒言う
stop [すべてをとめる v]
end
```

この新しいコードは`ずっと`{:class="block3control"} ループ内になければならないことを忘れないようにしてください。

--- /hint ------ /hints --- --- /task ---