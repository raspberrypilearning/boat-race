## Chiến thắng!

\--- task \--- Bây giờ thêm một câu lệnh `if`{: class = "block3control"} vào mã sprite thuyền của bạn để người chơi chiến thắng khi họ đưa thuyền đến đảo vàng.

Khi thuyền đến đảo, trò chơi sẽ nói 'YEAH!', Và rồi nó sẽ kết thúc.

\--- gợi ý \--- \--- gợi ý \--- Bạn cần thêm nhiều khối mã bên trong vòng lặp `mãi mãi`{: class = "block3control"} để mã của bạn tiếp tục kiểm tra xem người chơi đã thắng chưa:

`nếu`{: class = "block3control"} thuyền là `chạm`{: class = "block3sensing"} màu sắc của hòn đảo này, bạn cần phải `'! YEAH' nói trong 2 giây`{: class = "block3looks"} và sau đó `dừng tất cả`{: class = "block3control"} để kết thúc trò chơi. \--- / gợi ý \--- \--- gợi ý \--- Đây là các khối mã bạn cần: ![thuyền-sprite](images/boat_resize.png)

```blocks3
nói [YEAH!] trong (2) giây

nếu <touching color [#FFFF99] ?> thì
kết thúc

dừng [tất cả v]

```

\--- / gợi ý \--- \--- gợi ý \--- Đây là mã mới của bạn sẽ như thế nào: ![thuyền-sprite](images/boat_resize.png)

```blocks3
nếu <touching color [#FFFF99] ?> thì
nói [YEAH!] trong (2) giây
dừng [tất cả v]
kết thúc
```

Đừng quên rằng mã mới này cần nằm trong vòng lặp `mãi mãi`{: class = "block3control"}. \--- / gợi ý \--- \--- / gợi ý \--- \--- / nhiệm vụ \---