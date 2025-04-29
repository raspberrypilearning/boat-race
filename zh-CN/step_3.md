## 控制赛艇

\--- task \---

Add this code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![艇角色](images/boat_resize.png)

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

单击绿色旗帜并移动鼠标来**测试代码** 。艇角色是否向鼠标指针移动？

![截屏](images/boat-mouse.png)

\--- no-print \---

![截屏](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![截屏](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

当艇到达鼠标指针时会发生什么？试试看看问题是什么。

\--- /task \---

\--- task \---

Add code to the boat sprite so it only point towards the mouse pointer and moves `if`{:class="block3control"} the `distance to the mouse pointer`{:class="block3sensing"} is `greater than 5 pixels`{:class="block3operators"}.

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
+if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

\--- /task \---

\--- task \---

再次测试你的代码看问题现在是否已修复。

\--- /task \---