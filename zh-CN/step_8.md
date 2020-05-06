## 障碍物和助推器

现在游戏是 **太** 太容易了，所以你会添加一些东西，使它更有趣。

首先，你将添加一些助推器来给艇加速。

--- task ---

通过添加一些白色助推器箭头来编辑您的舞台背景。

![截图](images/boat-boost.png)

--- /task ---

--- task ---

现在添加更多的代码块，你的船的 `重复执行`{:class="block3control"}循环，使艇角色触碰到白色箭头时多移动3步。

![艇角色](images/boat_resize.png)

```blocks3
if <touching color [#FFFFFF] ?> then
move (3) steps
end
```

--- /task ---

--- task ---

测试你的游戏，看看你的新助推器是否让艇加速了。

--- /task ---

接下来，您将添加艇必须要避开的旋转门。

--- task ---

添加一个看起来像这样的新角色，并将其命名为'门'：

![截屏](images/boat-gate.png)

确保门角色的颜色与木质障碍物的颜色相同。

![截屏](images/brown-hsv.png)

--- /task ---

--- task ---

确保门角色的中心位于中间。

![截屏](images/boat-center.png)

--- /task ---

--- task ---

添加代码到你的门角色，使其永远缓慢旋转。

--- hints ---
 --- hint ---

向门精灵添加代码块，使其`转1度`{:class="block3motion"} `永远`{:class="block3control"}。

--- /hint --- --- hint ---

以下是你需要的代码块：

![门](images/gate.png)

```blocks3
forever
end

turn cw (1) degrees

when flag clicked
```

--- /hint --- --- hint ---

您的代码看起来应该是这样的：

![门](images/gate.png)

```blocks3
when flag clicked
forever
turn cw (1) degrees
end
```

--- /hint ------ /hints ---

--- /task ---

--- task ---

再次测试你的游戏。现在应该有一个旋转门，你需要控制你的船通过它。

![截屏](images/boat-gate-test.png)

--- /task ---