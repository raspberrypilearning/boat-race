## 添加计时器

现在，您将为游戏添加计时器，以便玩家必须尽快到达岛屿。

\--- task \---

在舞台上添加一个名为 `时间`{:class =“block3variables”}的新变量。

![截屏](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

您还可以通过更改新变量的显示方式来选择计时器外观。

\--- /task \---

\--- task \---

现在将代码块添加到舞台上，以便计时器计时，直到船到达岛屿。

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
change [time v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [time v] to [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
when flag clicked
set [time v] to [0]
forever
wait (0.1) seconds
change [time v] by (0.1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---