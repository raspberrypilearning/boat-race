## 控制船只

玩家将用鼠标控制船角色。

\--- task \--- 将代码添加到船角色中，使其从左下角开始向上，然后跟随鼠标指针。

![船角色](images / boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
point towards (mouse-pointer v)
move (1) steps
```

\--- /task \---

\--- task \---

单击绿色旗帜并移动鼠标来**测试代码** 。船是否向鼠标指针移动？

![截屏](images/boat-mouse.png)

\--- no-print \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- /no-print \---

\--- print-only \--- ![screenshot](images/boat-pointer-test-anim.png) \--- /print-only \---

\--- /task \---

\--- task \---

当船到达鼠标指针时会发生什么？试试看看问题是什么。

\--- /task \---

\--- task \---

要阻止这种情况发生，你需要在你的代码中添加一个 `if`{class =“block3control”}块，这样只有当它与鼠标指针相距超过5个像素时船才会移动。

\--- hints \--- \--- hint \--- 船应该指向鼠标指针并移动 `如果`{:class =“block3control”} `距离鼠标指针`{:class = “block3sensing”}是 `大于5个像素`{:class= “block3operators”}。 \--- /hint \--- \--- hint \--- 这些是您需要添加到船角色代码中的代码块： ![船角色](images / boat_resize.png)

```blocks3
if < [ ] > [ ] > then

(distance to (mouse-pointer v))
```

\--- /hint \--- \--- hint \--- 你的代码应该像这样：![船角色](images / boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

再次测试您的代码看问题现在是否已修复。

\--- /task \---