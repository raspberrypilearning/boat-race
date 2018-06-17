## 控制赛艇

\--- task \---

你需要用鼠标控制赛艇。 为赛艇添加代码让它从舞台左下角向上出发然后跟随鼠标指针移动。 **测试你的代码**以确保它按照预期正常工作。

\--- hints \--- \--- hint \--- 一旦`绿旗被点击`，你需要将赛艇`移到出发位置`并`面向上`。 然后赛艇需要`面向鼠标指针`并`移动1步`。 `重复执行`上面的过程。

\--- /hint \--- \--- hint \--- 这是你需要用到的代码块： ![screenshot](images/boat-move-blocks.png) \--- /hint \--- \--- hint \--- 你的代码应该如下图这样： ![screenshot](images/boat-move-code.png) \--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

点击绿旗并移动鼠标来测试你的赛艇。赛艇会向着鼠标航行吗？

![screenshot](images/boat-mouse.png)

![screenshot](images/boat-pointer-test-anim.gif)

## \--- collapse \---

title: 如果你遇到了困难...

## image: images/image.png

**注意：**目前Scratch有bug，可能会导致你的赛艇不会向着鼠标指针移动。 If this happens, click the arrow on the `point towards` block and re-select `mouse-pointer`.

![screenshot](images/boat-bug.png) \--- /collapse \---

\--- /task \---

\--- task \---

What happens if the boat reaches the mouse pointer? Try it.

\--- /task \---

\--- task \---

To stop this from happening, you'll need to add an `if` block to your code, so that the boat only moves if it is more than 5 pixels away from the mouse.

\--- hints \--- \--- hint \--- The boat should only point towards the mouse pointer and move `if` the `distance to the mouse pointer` is `greater than 5 pixels`. \--- /hint \--- \--- hint \--- Here are the code blocks you'll need to add to the code for the boat: ![screenshot](images/boat-pointer-blocks.png) \--- /hint \--- \--- hint \--- This is what your code should look like: ![screenshot](images/boat-pointer-code.png) \--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your boat again to check whether the problem has been fixed.

\--- /task \---