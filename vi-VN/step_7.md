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

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
thay đổi [thời gian v] bằng (0,1)

khi cờ nhấp

mãi mãi
kết thúc

chờ (0,1) giây

đặt [thời gian v] thành [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

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

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---