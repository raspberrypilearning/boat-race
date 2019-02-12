## 贏了！

\---任務- 現在添加一個 `如果`{：類=“block3control”}聲明你的船精靈的代碼，這樣的玩家獲勝時，他們使船在黃海島到達。

當船到達島嶼時，遊戲應該說'YEAH！'，然後它應該結束。

\---提示\--- \---提示\--- 您需要在 `永久`{：class =“block3control”}循環中添加更多代碼塊，以便您的代碼繼續檢查玩家是否贏了：

`如果`{{class =“block3control”}船是 `接觸`{{class =“block3sensing”}島的顏色，你需要 `說'YEAH！'持續2秒`{：class =“block3looks”}然後 `停止所有`{：class =“block3control”}以結束遊戲。 \--- /提示\--- \---提示\--- 以下是您需要的代碼塊： ![船精靈](images/boat_resize.png)

```blocks3
說[YEAH！]為（2）秒

如果 <touching color [#FFFF99] ?> 然後
結束

停止[全v]

```

\--- /提示\--- \---提示\--- 這是你的新代碼應該是什麼樣子： ![船精靈](images/boat_resize.png)

```blocks3
如果 <touching color [#FFFF99] ?> 然後
說[YEAH！]為（2）秒
停止[全v]
結束
```

不要忘記這個新代碼需要在 `永遠`{：class =“block3control”}循環中。 \--- /提示\--- \--- /提示\--- \--- /任務\---