## 添加计时器

现在，您将为游戏添加计时器，以便玩家必须尽快到达岛屿。

\--- task \---

在舞台上添加一个名为 `time`{：class =“block3variables”}的新变量。

![截屏](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

您还可以通过更改新变量的显示方式来选择查找计时器。

\--- /task \---

\--- task \---

现在将代码块添加到舞台上，以便计时器计时，直到船到达岛屿。

\---提示\--- \---提示\--- 在舞台上， `点击绿色标志时`{：class =“block3control”}， `将时间设置为0`{：class =“block3variables “}。 里面的 `永远`{：类= “block3control”}循环，你需要先 `等待0.1秒`{：类= “block3control”}，然后 `改变的时间由0.1`{：类= “block3variables” }。 \--- /提示\--- \---提示\--- 以下是您需要的代码块： ![阶段](images/stage.png)

```blocks3
当标志点击

永久
结束

等待（0.1）秒

设置[时间v]到 [0]时，将[时间v]改变为（0.1）


```

\--- /提示\--- \---提示\--- 这是你的新代码应该是什么样子： ![阶段](images/stage.png)

```blocks3
当标记点击时
设置[时间v]到 [0]
永远
等待（0.1）秒
改变[时间v]乘以（0.1）
结束
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

测试你的游戏，看看你有多快把船送到岛上！

![截屏](images/boat-variable-test.png)

\--- /task \---