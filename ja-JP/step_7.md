## タイマーの追加

次に、ゲームにタイマーを追加して、プレーヤーができるだけ早く島に着かなければならないようにしましょう。

--- task ---

`時間`{:class="block3variables"}という新しい変数をステージに追加します。

![スクリーンショット](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

新しい変数の表示方法を変更して、タイマーの外観を選択することもできます。

--- /task ---

--- task ---

ボートが島に到着するまでタイマーがカウントアップするように、ステージにコードブロックを追加します。

--- hints ---
 --- hint ---

ステージで、`緑の旗がクリックされたら`{:class="block3control"} 、`時間を０にします`{:class="block3variables"}。 `ずっと`{:class="block3control"}ループ内で、まず`0.1秒待って`{:class="block3control"}、`時間を 0.1秒ずつ変化させます`{:class="block3variables"}。

--- /hint --- --- hint ---

必要なコードブロックは次のとおりです。

![ステージ](images/stage.png)

```blocks3
[時間 v] を (0.1) ずつ変える

⚑ が押されたとき

ずっと
end

(0.1) 秒待つ

[時間 v] を [0] にする
```

--- /hint --- --- hint ---

新しいコードは次のようになります。

![ステージ](images/stage.png)

```blocks3
⚑ が押されたとき
[時間 v] を [0] にする
ずっと 
(0.1) 秒待つ
[時間 v] を (0.1) ずつ変える
end
```

--- /hint ------ /hints ---

--- /task ---

--- task ---

ゲームを試して、どれだけ早くボートを無人島にたどり着かせることができるか確かめましょう！

![スクリーンショット](images/boat-variable-test.png)

--- /task ---