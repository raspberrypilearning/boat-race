## 障碍和助力

目前，这个游戏_太_容易了 - 让我们来添加一些内容，使其更加有趣。

+ 让我们首先向你的游戏添加一些“助力器”来使船只加速。编辑你的工作区背景，加入一些白色的助力器箭头。

	![screenshot](images/boat-boost.png)

+ 现在向你船只的永远循环添加一些代码，使其碰到白色助力器就能多移动三步。

--- hints ---
--- hint ---
`如果` 你的船只 `触碰白色助力器` ，则其应 `多移动 3 步`。  
--- /hint ---
--- hint ---
以下是你将需要的代码块：
![screenshot](images/boat-boost-blocks.png)
--- /hint ---
--- hint ---
你的代码应如下所示：
![screenshot](images/boat-boost-code.png)
--- /hint ---
--- /hints ---

+ 你还可以添加一个船只必须避开的旋转门。添加一个被称作“门”的新子图，如下所示：

	![screenshot](images/boat-gate.png)

	确保门的颜色与木头障碍的颜色相同。

+ 设置门子图的中心。

	![screenshot](images/boat-center.png)

+ 向你的门添加代码，使其能永远缓慢旋转。

--- hints ---
--- hint ---
向门子图添加代码，使其 `永远` `转 1 度`。
--- /hint ---
--- hint ---
以下是你将需要的代码块：
![screenshot](images/boat-spin-blocks.png)
--- /hint ---
--- hint ---
你的代码应如下所示：
![screenshot](images/boat-spin-code.png)
--- /hint ---
--- /hints ---


+ 测试你的游戏。你现在应该有了一个你必须避开的旋转门。

	![screenshot](images/boat-gate-test.png)
