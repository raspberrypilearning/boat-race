## 控制船隻

\--- task \---

Add this code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![船隻角色](images/boat_resize.png)

```blocks3
當 @greenflag 被點擊
面朝 (0) 度
定位到 x:(-190) y:(150)
重複無限次
面朝 (鼠標 v) 向
移動 (1) 點
end
```

\--- /task \---

\--- task \---

點擊綠旗**測試你的程式**，動動滑鼠，船隻會朝著鼠標位置的方向移動嗎？

![截圖](images/boat-mouse.png)

\--- no-print \---

![截圖](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![截圖](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

當船隻到了鼠標的位置時會發生什麼事？試一試，看看問題出在哪兒。

\--- /task \---

\--- task \---

Add code to the boat sprite so it only point towards the mouse pointer and moves `if`{:class="block3control"} the `distance to the mouse pointer`{:class="block3sensing"} is `greater than 5 pixels`{:class="block3operators"}.

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
+if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

\--- /task \---

\--- task \---

再試一下程式，看看問題是不是解決了。

\--- /task \---