## 添加計時器

在遊戲裡添加計時工具，看看玩家能多快抵達小島。

\--- task \---

在舞台上添加一個名為 `計時`{:class="block3variables"} 的新變數。

![截圖](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

你可以在舞台上顯示的變數上右擊滑鼠，選擇變數顯示的樣式。

\--- /task \---

\--- task \---

現在我們編寫舞台的程式，讓計時器在背景計算時間，看船隻什麼時候到達小島。

\--- hints \--- \--- hint \---

只要`一點擊綠旗`{:class="block3control"} ，舞台背景的`計時就先重設回 0`{:class="block3variables"}。 接著計時工具上的數字就開始`不斷重複`{:class="block3control"} 的 `每經過 0.1 秒`{:class="block3control"} 就`加 0.1 `{:class="block3variables"}。

\--- /hint \--- \--- hint \---

這裡是你需要的程式積木：

![舞台](images/stage.png)

```blocks3
變數 [計時 v] 改變 (0.1)

當 @greenflag 被點擊

重複無限次
end

等待 (0.1) 秒

變數 [計時 v] 設為 (0)
```

\--- /hint \--- \--- hint \---

你的程式看起來應該像這樣：

![舞台](images/stage.png)

```blocks3
當 @greenflag 被點擊
變數 [計時 v] 設為 (0)
重複無限次
等待 (0.1) 秒
變數 [計時 v] 改變 (0.1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

測試你的遊戲，看看你自己能多快讓船隻開往小島！

![截圖](images/boat-variable-test.png)

\--- /task \---