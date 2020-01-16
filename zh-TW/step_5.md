## 贏了！

\--- task \---

Now add another `if`{:class="block3control"} statement to your boat sprite's code so that the player wins when they make the boat arrive at the yellow island.

When the boat gets to the island, the game should say 'YEAH!', and then it should end.

\--- hints \--- \--- hint \---

You need to add more code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the player has won:

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the colour of the island, you need to `say 'YEAH!' for 2 seconds`{:class="block3looks"} and then `stop all`{:class="block3control"} to end the game.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
說[YEAH！]為（2）秒

如果 <touching color [#FFFF99] ?> 然後
結束

停止[全v]

```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
如果 <touching color [#FFFF99] ?> 然後
說[YEAH！]為（2）秒
停止[全v]
結束
```

Don't forget that this new code needs to be inside the `forever`{:class="block3control"} loop.

\--- /hint \--- \--- /hints \--- \--- /task \---