## 撞击!

目前，你的赛艇还可以穿过木栅栏！我们来修复这个问题。

\--- task \---

你的赛艇需要2个造型，一个正常造型，一个撞击造型。复制赛艇造型，将一个命名为“正常”另一个命名为“撞击”。

\--- /task \---

\--- task \---

Click on your 'hit' costume, and choose the Select tool to grab bits of the boat and move and rotate them around to make it look as if it's crashed.

![screenshot](images/boat-hit-costume.png)

\--- /task \---

\--- task \---

Now add code to your boat so that it crashes and breaks up when it touches any brown wooden bits.

\--- hints \--- \--- hint \--- You need to add code inside your `forever` loop so that your code keeps checking if the boat has crashed. `If` the boat is `touching` the brown colour of the wood, you need to `switch to the hit costume`, `say Noooo! for 2 seconds`, and then `switch back to the normal costume`. Finally, you'll need to `point up` and `go to the start position`. \--- /hint \--- \--- hint \--- Here are the code blocks you'll need: ![screenshot](images/boat-hit-blocks.png) \--- /hint \--- \--- hint \--- Here's what your code should look like: ![screenshot](images/boat-hit-code.png) \--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also make sure that your boat always starts out looking 'normal'.

If you try to sail through a wooden barrier now, you should see that your boat crashes and moves back to the start.

![screenshot](images/boat-crash.png)

\--- /task \---