## Thêm một bộ đếm thời gian

Bây giờ bạn sẽ thêm một bộ đếm thời gian vào trò chơi của mình, để người chơi phải đến đảo càng nhanh càng tốt.

\--- task \---

Thêm một biến mới có tên `time`{: class = "block3variables"} vào Giai đoạn của bạn.

![ảnh chụp màn hình](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Bạn cũng có thể chọn giao diện cho bộ đếm thời gian của mình bằng cách thay đổi cách hiển thị biến mới của bạn.

\--- /bài tập \---

\--- task \---

Bây giờ thêm các khối mã vào Giai đoạn của bạn để bộ đếm thời gian đếm ngược cho đến khi thuyền đến đảo.

\--- gợi ý \--- \--- gợi ý \--- Trên sân khấu, `khi cờ xanh được nhấp`{: class = "block3control"}, `đặt thời gian thành 0`{: class = "block3variabled "}. Bên trong vòng lặp `mãi mãi`{: class = "block3control"}, trước tiên bạn sẽ cần `giây chờ 0,1 giây`{: class = "block3control"}, sau đó `thay đổi thời gian bằng 0,1`{: class = "block3variables" }. \--- / gợi ý \--- \--- gợi ý \--- Đây là các khối mã bạn cần: ![sân khấu](images/stage.png)

```blocks3
thay đổi [thời gian v] bằng (0,1)

khi cờ nhấp

mãi mãi
kết thúc

chờ (0,1) giây

đặt [thời gian v] thành [0]
```

\--- / gợi ý \--- \--- gợi ý \--- Đây là mã mới của bạn sẽ như thế nào: ![sân khấu](images/stage.png)

```blocks3
khi cờ nhấp
đặt [thời gian v] thành [0]
mãi mãi
chờ (0,1) giây
thay đổi [thời gian v] bằng (0,1)
kết thúc
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Kiểm tra trò chơi của bạn và xem bạn có thể nhanh chóng đưa thuyền đến đảo như thế nào!

![ảnh chụp màn hình](images/boat-variable-test.png)

\--- /bài tập \---