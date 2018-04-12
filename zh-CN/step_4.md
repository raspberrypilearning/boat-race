## 控制船只

+ 你将使用鼠标控制船只。向你的船只添加代码，使其从左下角朝上出发，然后跟随鼠标指针。__测试你的代码__以确保其发挥应有的作用。

--- hints ---
--- hint ---
`点击绿色旗帜` 后，你将需要使你的船只 `前往起始位置` 并 `朝上`。接下来，船只需要 `朝向鼠标指针` 并 `移动 1 步`。船只将需要 `永远` 重复此动作。

--- /hint ---
--- hint ---
以下是你将需要的代码块：
![screenshot](images/boat-move-blocks.png)
--- /hint ---
--- hint ---
你的代码应如下所示：
![screenshot](images/boat-move-code.png)
--- /hint ---
--- /hints ---

+ 通过点击旗帜和移动鼠标来测试你的船只。船只是否驶向鼠标？

	![screenshot](images/boat-mouse.png)

	![screenshot](images/boat-pointer-test-anim.gif)

--- collapse ---
---
title: 如果你有问题 ...
image: images/image.png
---
__注意：__Scratch 中目前存在一个错误，这意味着你的船只可能不会朝鼠标指针移动。如果发生这种情况，点击 `朝向` 模块上的箭头，重新选择 `鼠标指针`。

![screenshot](images/boat-bug.png)
--- /collapse ---


+ 如果船只到达鼠标指针位置会发生什么呢？试试看。

+ 为防止这种情况发生，你需要向你的代码添加 `如果` 模块，这样船只只有在距鼠标 5 个以上像素时才会移动。

--- hints ---
--- hint ---
`如果` `到鼠标指针的距离` `大于 5 个像素` ，船只方可朝向鼠标指针并移动。
--- /hint ---
--- hint ---
以下是你需要向船只代码添加的代码块：
![screenshot](images/boat-pointer-blocks.png)
--- /hint ---
--- hint ---
你的代码应如下所示：
![screenshot](images/boat-pointer-code.png)
--- /hint ---
--- /hints ---

+ 再次测试你的船只，检查问题是否已解决。
