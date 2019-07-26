## 控制赛艇

玩家将用鼠标控制船只精灵。

\--- task \--- 将代码添加到船精灵中，使其从左下角开始向上，然后跟随鼠标指针。

![船精灵](images/boat_resize.png)

```blocks3
当标志点击
点方向（0）
转到x：（-190）y：（ -  150）
永远
点朝（鼠标指针v）
移动（1）步
```

\--- /task \---

\--- task \---

**单击绿色标记并移动鼠标，测试代码** 。船精灵是否向鼠标指针移动？

![截屏](images/boat-mouse.png)

\---无印刷\--- ![screenshot](images/boat-pointer-test-anim.gif) \--- /无印刷\---

\---仅打印\--- ![screenshot](images/boat-pointer-test-anim.png) \--- /仅打印\---

\--- /task \---

\--- task \---

当船到达鼠标指针时会发生什么？试试看看问题是什么。

\--- /task \---

\--- task \---

要阻止这种情况发生，你需要在你的代码中添加一个 `{`class =“block3control”}块，这样只有当它与鼠标指针相距超过5个像素时才会移动。

\---提示\--- \---提示\--- 船只应指向鼠标指针并移动 `如果`{：class =“block3control”} `距离鼠标指针`{：class = “block3sensing”}是 `大于5个像素`{：类= “block3operators”}。 \--- /提示\--- \---提示\--- 这些是您需要添加到船精灵代码中的代码块： ![船精灵](images/boat_resize.png)

```blocks3
如果 < [] > [] > 然后

（距离（鼠标指针v））
```

\--- /hint \--- \--- hint \--- 你的代码应该像这样：![船精灵](images/boat_resize.png)

```blocks3
当标志点击
点方向（0）
转到x：（-190）y：（ -  150）
永远
如果 <（距离（鼠标指针v）） > [5]> 然后
点朝（鼠标 -指针v）
移动（1）步
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

再次测试您的代码以检查问题现在是否已修复。

\--- /task \---