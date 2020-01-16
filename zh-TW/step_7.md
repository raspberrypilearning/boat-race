## 添加計時器

現在，您將為遊戲添加計時器，以便玩家必須盡快到達島嶼。

\---任務\---

在舞台上添加一個名為 `time`{：class =“block3variables”}的新變量。

![截圖](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

您還可以通過更改新變量的顯示方式來選擇查找計時器。

\--- /任務\---

\---任務\---

現在將代碼塊添加到舞台上，以便計時器計時，直到船到達島嶼。

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
當標誌點擊

永久
結束

等待（0.1）秒

設置[時間v]到 [0]時，將[時間v]改變為（0.1）


```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
當標記點擊時
設置[時間v]到 [0]
永遠
等待（0.1）秒
改變[時間v]乘以（0.1）
結束
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---