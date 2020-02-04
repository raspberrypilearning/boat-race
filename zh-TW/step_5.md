## 到終點啦！

\--- task \---

現在添加另一個`如果`{:class="block3control"}陳述式船隻角色裡，當船隻到達黃色沙漠小島時，玩家獲得勝利。

當到達小島時，船隻會說出「到終點啦！」，然後遊戲結束。

\--- hints \--- \--- hint \---

你需要添加更多的程式到 `重複無限次`{:class="block3control"} 迴圈積木，以便不斷的檢查玩家是否獲勝：

`如果`{:class="block3control"} 船隻 `碰到`{:class="block3sensing"} 黃色的小島，就 `說出「到終點啦！」2 秒`{:class="block3looks"} ，然後 `停止全部`{:class="block3control"} 結束遊戲。

\--- /hint \--- \--- hint \---

這裡是你需要的程式積木：

![船隻角色](images/boat_resize.png)

```blocks3
說出 (到終點啦！) 持續 (2) 秒

如果 <碰到顏色 (#FFFF99)？> 那麼
end

停止 [全部 v]

```

\--- /hint \--- \--- hint \---

你的程式看起來應該像這樣：

![船隻角色](images/boat_resize.png)

```blocks3
如果 <碰到顏色 (#FFFF99)？> 那麼
說出 (到終點啦！) 持續 (2) 秒
停止 [全部 v]
end
```

注意這個新程式要放到迴圈積木`重複無限次`{:class="block3control"}裡。

\--- /hint \--- \--- /hints \--- \--- /task \---