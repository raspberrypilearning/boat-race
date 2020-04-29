## 添加计时器

现在，您将为游戏添加计时器，以便玩家必须尽快到达岛屿。

\--- task \---

在舞台上添加一个名为 `时间`{:class =“block3variables”}的新变量。

![截屏](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

您还可以通过更改新变量的显示方式来选择计时器外观。

\--- /task \---

\--- task \---

现在将代码块添加到舞台上，以便计时器计时，直到船到达岛屿。

\--- hints \--- \--- hint \---

在舞台上， `当点击绿色旗帜时`{:class =“block3control”}， `将时间设置为0`{:class =“block3variables “}。 在 `forever`{:class= “block3control”}循环里，你需要先 `等待0.1秒`{:class= “block3control”}，然后 `时间按每次0.1改变`{:class= “block3variables”}。

\--- /hint \--- \--- hint \---

以下是你需要的代码块：

![舞台](images/stage.png)

```blocks3
change [time v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [time v] to [0]
```

\--- /hint \--- \--- hint \---

您的代码看起来应该是这样的：

![舞台](images/stage.png)

```blocks3
when flag clicked
set [time v] to [0]
forever
wait (0.1) seconds
change [time v] by (0.1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

测试你的游戏，看看你能多快把艇送到岛上！

![截屏](images/boat-variable-test.png)

\--- /task \---