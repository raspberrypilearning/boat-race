## Điều khiển thuyền

Người chơi sẽ điều khiển thuyền sprite bằng chuột.

\--- task \--- Thêm mã vào sprite thuyền để nó bắt đầu ở góc dưới bên trái chỉ lên và sau đó theo con trỏ chuột.

![thuyền-sprite](images/boat_resize.png)

```blocks3
khi cờ nhấp
điểm theo hướng (0)
đi đến x: (-190) y: (-150)
mãi mãi
điểm về phía (con trỏ chuột v)
bước (1) bước
```

\--- /task \---

\--- task \---

**Kiểm tra mã của bạn** bằng cách nhấp vào cờ xanh và di chuyển chuột. Thuyền sprite có di chuyển về phía con trỏ chuột không?

![ảnh chụp màn hình](images/boat-mouse.png)

\--- không in \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- / không in \---

\--- chỉ in \--- ![screenshot](images/boat-pointer-test-anim.png) \--- / chỉ in \---

\--- /task \---

\--- task \---

Điều gì xảy ra khi thuyền đến con trỏ chuột? Hãy thử nó để xem vấn đề là gì.

\--- /task \---

\--- task \---

Để ngăn điều này xảy ra, bạn cần thêm một khối `nếu`{: class = "block3control"} vào mã của bạn, để sprite thuyền chỉ di chuyển nếu nó cách con trỏ chuột hơn 5 pixel.

\--- gợi ý \--- \--- gợi ý \--- Thuyền chỉ nên hướng về phía con trỏ chuột và di chuyển `nếu`{: class = "block3control"} khoảng cách `đến con trỏ chuột`{: class = "block3sensing"} là `lớn hơn 5 pixel`{: class = "block3operators"}. \--- / gợi ý \--- \--- gợi ý \--- Đây là các khối mã bạn cần thêm vào mã cho sprite thuyền: ![thuyền-sprite](images/boat_resize.png)

```blocks3
if < [] > [] > thì

(khoảng cách đến (con trỏ chuột v))
```

\--- / gợi ý \--- \--- gợi ý \--- Đây là mã của bạn sẽ như thế nào: ![thuyền-sprite](images/boat_resize.png)

```blocks3
khi cờ nhấp
điểm theo hướng (0)
đi tới x: (-190) y: (-150)
mãi mãi
nếu <(khoảng cách đến (con trỏ chuột v)) > [5]> rồi
điểm về phía (chuột- con trỏ v)
bước (1) bước
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Kiểm tra lại mã của bạn để kiểm tra xem sự cố đã được khắc phục chưa.

\--- /task \---