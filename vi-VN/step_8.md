## Chướng ngại vật và tên lửa đẩy

Ngay bây giờ trò chơi là **xa** quá dễ dàng, vì vậy bạn sẽ thêm một số điều để làm cho nó thú vị hơn.

Đầu tiên, bạn sẽ thêm một số tên lửa đẩy để tăng tốc thuyền.

\--- task \---

Chỉnh sửa phông nền sân khấu của bạn bằng cách thêm vào một số mũi tên tăng cường màu trắng.

![ảnh chụp màn hình](images/boat-boost.png)

\--- /task \---

\--- task \---

Bây giờ thêm nhiều khối mã vào vòng lặp `của thuyền của bạn mãi mãi`{: class = "block3control"} để thuyền sprite di chuyển thêm ba bước khi chạm vào mũi tên trắng. ![thuyền-sprite](images/boat_resize.png)

```blocks3
nếu <touching color [#FFFFFF] ?> thì
di chuyển (3) bước
kết thúc
```

\--- /task \---

\--- task \---

Kiểm tra trò chơi của bạn để xem liệu mũi tên tăng cường mới của bạn tăng tốc thuyền.

\--- /bài tập \---

Tiếp theo bạn sẽ thêm một cổng quay mà thuyền phải tránh.

\--- task \---

Thêm một sprite mới trông như thế này và gọi nó là 'gate':

![ảnh chụp màn hình](images/boat-gate.png)

Hãy chắc chắn rằng màu sắc của sprite cổng giống với màu của hàng rào gỗ.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![cánh cổng](images/gate.png)

```blocks3
mãi mãi
kết thúc

lượt cw (1) độ

khi cờ được nhấp
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

```blocks3
khi cờ nhấp
mãi mãi
lượt cw (1) độ
kết thúc
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---