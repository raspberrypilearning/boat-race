## 胜利！

\--- task \---

现在添加另外一个 `如果`{:class=“block3control”}语句到你的艇角色的代码，这样当玩家的艇达到黄色海岛时获胜。

当船到达岛屿时，游戏应该说'耶!'，然后它应该结束。

\--- hints \--- \--- hint \---

您需要在 `forever`{:class =“block3control”}循环中添加更多代码块，以便您的代码继续检查玩家是否赢了：

`如果`{:class =“block3control”}艇 `接触到`{:class =“block3sensing”}岛的颜色，你需要 `说'耶!'持续2秒`{:class =“block3looks”}然后 `停止所有`{:class =“block3control”}以结束游戏。

\--- /hint \--- \--- hint \---

以下是你需要的代码块：

![艇角色](images/boat_resize.png)

```blocks3
say [YEAH!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

\--- /hint \--- \--- hint \---

您的代码看起来应该是这样的：

![艇角色](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
```

不要忘记这个新代码需要在 `forever`{:class =“block3control”}循环中。

\--- /hint \--- \--- /hints \--- \--- /task \---