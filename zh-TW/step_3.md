## 控制船隻

讓玩家能夠用滑鼠游標控制船隻角色。

\--- task \---

為船隻角色編寫程式，讓它從左下角開始，然後跟隨滑鼠游標的位置前進。

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

為了避免這種情況發生，你必須添加 `如果`{:class="block3control"} 積木到程式中，這樣一來，船隻角色只有在距離鼠標 5 點以上時才會動作。

\--- hints \--- \--- hint \---

船隻應該只會面朝滑鼠游標的位置，`如果`{:class="block3control"} 船隻 `與鼠標的間距`{:class="block3sensing"} `大於 5 點`{:class="block3operators"} 時才會移動。

\--- /hint \--- \--- hint \---

這些是船隻角色會用到的程式積木：

![船隻角色](images/boat_resize.png)

```blocks3
如果 <() > ()> 那麼 否則

與 (鼠標 v) 的間距
```

\--- /hint \--- \--- hint \---

你的程式看起來應該像這樣：

![船隻角色](images/boat_resize.png)

```blocks3
當 @greenflag 被點擊
面朝 (0) 度
定位到 x:(-190) y:(150)
重複無限次
如果 <(與 (鼠標 v) 的間距) > (5)> 那麼
面朝 (鼠標 v) 向
移動 (1) 點
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

再試一下程式，看看問題是不是解決了。

\--- /task \---