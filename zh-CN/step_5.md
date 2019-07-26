## 撞击

\---任务- 现在添加一个 `如果`{：类=“block3control”}声明你的船精灵的代码，这样的玩家获胜时，他们使船在黄海岛到达。

当船到达岛屿时，游戏应该说'YEAH！'，然后它应该结束。

\---提示\--- \---提示\--- 您需要在 `永久`{：class =“block3control”}循环中添加更多代码块，以便您的代码继续检查玩家是否赢了：

`如果`{{class =“block3control”}船是 `接触`{{class =“block3sensing”}岛的颜色，你需要 `说'YEAH！'持续2秒`{：class =“block3looks”}然后 `停止所有`{：class =“block3control”}以结束游戏。 \--- /提示\--- \---提示\--- 以下是您需要的代码块： ![船精灵](images/boat_resize.png)

```blocks3
说[YEAH！]为（2）秒

如果 <touching color [#FFFF99] ?> 然后
结束

停止[全v]

```

\--- /提示\--- \---提示\--- 这是你的新代码应该是什么样子： ![船精灵](images/boat_resize.png)

```blocks3
如果 <touching color [#FFFF99] ?> 然后
说[YEAH！]为（2）秒
停止[全v]
结束
```

不要忘记这个新代码需要在 `永远`{：class =“block3control”}循环中。 \--- /提示\--- \--- /提示\--- \--- /任务\---