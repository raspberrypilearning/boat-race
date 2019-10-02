## 计时赛

现在游戏是 **远** 太容易了，所以你会添加一些东西，使它更有趣。

首先，你将添加一些助推器来加速船。

\---任务\---

通过添加一些白色助推器箭头来编辑您的舞台背景。

![截图](images/boat-boost.png)

\--- /任务\---

\--- task \---

现在添加更多的代码块，你的船的 `永远`{:class=“block3control”}循环，使艇精灵移动三个额外的步骤时，倒是一个白色箭头。 ![船精灵](images/boat_resize.png)

```blocks3
如果 <touching color [#FFFFFF] ?> 然后
移动（3）步骤
结束
```

\--- /任务\---

\---任务\---

测试你的游戏，看看你的新助推器是否加速了船。

\--- /任务\---

接下来，您将添加船只必须避免的旋转门。

\---任务\---

添加一个看起来像这样的新精灵，并将其命名为'gate'：

![截图](images/boat-gate.png)

确保门精灵的颜色与木质障碍物的颜色相同。

![截图](images/brown-hsv.png)

\---任务\---

\---任务\---

确保门精灵的中心位于中间。

![screenshot](images/boat-center.png)

\--- /任务\---

\---任务\---

添加代码到您的门精灵，使其永远缓慢旋转。

\---提示集\--- \---提示\--- 向门精灵添加代码块，使其`转1度` {：class =“block3motion”} `永远` {：类= “block3control”}。 \--- /提示\--- \---提示\--- 以下是您需要的代码块： ![门](images/gate.png)

```blocks3
forever
end

turn cw (1) degrees

when flag clicked

```

\--- /提示\--- \---提示\--- 这是你的新代码的样子： ![门](images/gate.png)

```blocks3
when flag clicked
forever
turn cw (1) degrees
end
```

\--- /提示\--- \--- /提示集\---

\--- /任务\---

\---任务\---

再次测试你的游戏。你现在应该有一个旋转门，你需要搅动你的船。

![截图](images/boat-gate-test.png)

\--- /任务\---