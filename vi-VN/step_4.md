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

\--- gợi ý \--- \--- gợi ý \--- Bạn cần thêm các khối mã bên trong vòng lặp `mãi mãi`{: class = "block3control"} để mã của bạn tiếp tục kiểm tra xem sprite thuyền có bị hỏng hay không và nếu nó bị hỏng, mã cần thiết lập lại vị trí của thuyền sprite.

`nếu`{: class = "block3control"} thuyền là `chạm`{: class = "block3sensing"} màu nâu của gỗ, bạn cần phải `chuyển sang trang phục hit`{: class = "block3looks"} , `nói Noooo! trong 2 giây`{: class = "block3looks"} và sau đó `chuyển trở lại trang phục bình thường`{: class = "block3looks"}. Cuối cùng, bạn sẽ cần `điểm lên`{: class = "block3motion"} và `đi đến vị trí bắt đầu`{: class = "block3motion"}.

\--- / gợi ý \--- \--- gợi ý \--- Đây là các khối mã bạn cần: ![thuyền-sprite](images/boat_resize.png)

```blocks3
nếu <touching color [ ] ?> thì
kết thúc

đi đến x: (-190) y: (-150)

chuyển trang phục sang (nhấn v)

điểm theo hướng (0)

chuyển trang phục sang (bình thường v)

nói [Noooooo!] cho (2 giây
```

\--- / gợi ý \--- \--- gợi ý \--- Đây là mã của bạn sẽ như thế nào: ![thuyền-sprite](images/boat_resize.png)

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

\--- /task \---

\--- task \---

Bạn cũng nên thêm mã để đảm bảo rằng sprite thuyền của bạn luôn bắt đầu trông 'bình thường'.

Kiểm tra mã của bạn một lần nữa. Nếu bạn cố chèo thuyền qua một hàng rào gỗ bây giờ, thuyền sẽ gặp sự cố và sau đó di chuyển trở lại vị trí bắt đầu.

![ảnh chụp màn hình](images/boat-crash.png)

\--- /bài tập \---