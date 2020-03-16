## 胜利！

\--- task \---

现在添加一个 `if`{:class=“block3control”}声明你的船角色的代码，这样当玩家的船达到黄色海岛时获胜。

When the boat gets to the island, the game should say 'YEAH!', and then it should end.

\--- hints \--- \--- hint \---

您需要在 `forever`{:class =“block3control”}循环中添加更多代码块，以便您的代码继续检查玩家是否赢了：

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the colour of the island, you need to `say 'YEAH!' for 2 seconds`{:class="block3looks"} and then `stop all`{:class="block3control"} to end the game.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
say [YEAH!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

\--- /hint \--- \--- hint \---

您的代码看起来应该是这样的：

![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
```

不要忘记这个新代码需要在 `forever`{:class =“block3control”}循环中。

\--- /hint \--- \--- /hints \--- \--- /task \---