## 障礙和助推器

現在遊戲是 **遠** 太容易了，所以你會添加一些東西，使它更有趣。

首先，你將添加一些助推器來加速船。

\---任務\---

通過添加一些白色助推器箭頭來編輯您的舞台背景。

![截圖](images/boat-boost.png)

\--- /任務\---

\---任務\---

現在添加更多的代碼塊，你的船的 `永遠`{：類=“block3control”}循環，使艇精靈移動三個額外的步驟時，倒是一個白色箭頭。 ![船精靈](images/boat_resize.png)

```blocks3
如果 <touching color [#FFFFFF] ?> 然後
移動（3）步驟
結束
```

\--- /任務\---

\---任務\---

測試你的遊戲，看看你的新助推箭是否加速了船。

\--- /任務\---

接下來，您將添加船隻必須避免的旋轉門。

\---任務\---

添加一個看起來像這樣的新精靈，並將其命名為'gate'：

![截圖](images/boat-gate.png)

確保門精靈的顏色與木質障礙物的顏色相同。

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![門](images/gate.png)

```blocks3
永遠
結束

點擊標誌時轉cw（1）度


```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

```blocks3
當標誌點擊
永遠
轉cw（1）度
結束
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---