## Va chạm!

Tại thời điểm này, thuyền sprite có thể đơn giản đi thuyền qua các hàng rào bằng gỗ! Bây giờ bạn sẽ sửa nó.

\--- task \---

Bạn cần hai trang phục cho thuyền của bạn: một trang phục bình thường và một cho khi thuyền gặp sự cố. Sao y trang phục thuyền của bạn và đặt tên cho một trang phục là 'bình thường' và 'trang phục' khác.

\--- /bài tập \---

\--- task \---

Nhấp vào trang phục 'hit' của bạn và sử dụng công cụ **Chọn** để lấy các mảnh của trang phục và di chuyển và xoay chúng để làm cho chiếc thuyền trông giống như nó đã bị vỡ thành từng mảnh.

![ảnh chụp màn hình](images/boat-hit-costume-annotated.png)

\--- /bài tập \---

\--- task \---

Bây giờ thêm mã vào thuyền của bạn để nó gặp sự cố và vỡ khi chạm vào bất kỳ rào cản bằng gỗ màu nâu nào.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
nếu <touching color [ ] ?> thì
kết thúc

đi đến x: (-190) y: (-150)

chuyển trang phục sang (nhấn v)

điểm theo hướng (0)

chuyển trang phục sang (bình thường v)

nói [Noooooo!] cho (2 giây
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
khi cờ nhấp
điểm theo hướng (0)
đi tới x: (-190) y: (-150)
mãi mãi
nếu <(khoảng cách đến (con trỏ chuột v)) > [5]> rồi
điểm về phía (chuột- con trỏ v)
di chuyển (1) bước
kết thúc
nếu <touching color [#663b00] ?> rồi
chuyển trang phục sang (nhấn v)
nói [Noooooo!] trong (2) giây
chuyển trang phục sang (bình thường v)
điểm theo hướng (0)
đi đến x: (-190) y: (-150)
kết thúc
```

\--- /hint \--- \--- /hints \---

\--- /bài tập \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---