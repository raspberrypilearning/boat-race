## 障碍与助力

目前游戏*太过*简单--让我们增加些难度提高一下游戏的乐趣。

\--- task \---

首先我们为游戏加入一些“加速点”来提升赛艇的速度。比编辑舞台背景加入一些白色的加速箭头。

![screenshot](images/boat-boost.png)

\--- /task \---

\--- task \---

在赛艇的重复执行循环中加入一些代码让赛艇触碰到白色加速标志时速度提升3倍。

\--- hints \--- \--- hint \--- `如果`赛艇`碰到白色加速标志`，那么它应该`额外移动3步`。  
\--- /hint \--- \--- hint \--- 下面是你需要用到的代码块： ![screenshot](images/boat-boost-blocks.png) \--- /hint \--- \--- hint \--- 你的代码应该如下图这样： ![screenshot](images/boat-boost-code.png) \--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You can also add a spinning gate which your boat will have to avoid. Add a new sprite called 'gate' that looks like this:

![screenshot](images/boat-gate.png)

Make sure that the colour of the gate is the same as that of the wooden barriers.

\--- /task \---

\--- task \---

Set the center of the gate sprite.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code to the gate sprite so that it `turns 1 degree` `forever`. \--- /hint \--- \--- hint \--- Here are the code blocks you'll need: ![screenshot](images/boat-spin-blocks.png) \--- /hint \--- \--- hint \--- Here's what your code should look like: ![screenshot](images/boat-spin-code.png) \--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game. You should now have a spinning gate that you must avoid.

![screenshot](images/boat-gate-test.png)

\--- /task \---