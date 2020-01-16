## 崩潰！

此刻，船精靈可以簡單地穿過木柵欄！你現在要解決這個問題。

\---任務\---

你的船精靈需要兩件服裝：一件普通的服裝，一件用於船撞的時候。複製你的船精靈的服裝，並命名一個服裝'正常'和另一個'打'。

\--- /任務\---

\---任務\---

點擊你的“點擊”服裝，然後使用 **選擇** 工具抓住服裝的部分並移動和旋轉它們，使船看起來像是碎成碎片。

![截圖](images/boat-hit-costume-annotated.png)

\--- /任務\---

\---任務\---

現在將代碼添加到您的船上，以便在碰到任何棕色木質障礙物時崩潰並破碎。

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
如果 <touching color [ ] ?> 然後
結束

轉到x：（-190）y：（ -  150）

切換服裝到（點擊v）

點方向（0）

切換服裝到（正常v）

說[Noooooo！] for （2）秒
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
當標誌點擊
點方向（0）
轉到x：（-190）y：（ -  150）
永遠
如果 <（距離（鼠標指針v）） > [5]> 然後
點朝（鼠標 -指針v）
移動（1）步驟
結束
如果 <touching color [#663b00] ?> 然後
切換服裝到（擊中v）
說[Noooooo！]為（2）秒
開關服裝到（正常v）
點方向（0）
轉到x：（-190）y：（ -  150）
結束
```

\--- /hint \--- \--- /hints \---

\--- /任務\---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---