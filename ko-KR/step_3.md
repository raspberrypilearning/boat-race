## 배 조종하기

플레이어는 보트 스프라이트를 마우스로 제어합니다.

\--- task \---

Add code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![boat-sprite](images/boat_resize.png)

```blocks3
녹색 깃발이 클릭되었을 때
(0) 도 방향 보기
x: (-190) y: (-150) 으로 이동하기
무한 반복하기
(마우스 포인터 v) 쪽 보기
(1) 만큼 움직이기
```

\--- /task \---

\--- task \---

**Test your code** by clicking the green flag and moving the mouse. Does the boat sprite move towards the mouse pointer?

![screenshot](images/boat-mouse.png)

\--- no-print \---

![screenshot](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![screenshot](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

What happens when the boat reaches the mouse pointer? Try it out to see what the problem is.

\--- /task \---

\--- task \---

To stop this from happening, you need to add an `if`{:class="block3control"} block to your code, so that the boat sprite only moves if it is more than 5 pixels away from the mouse pointer.

\--- hints \--- \--- hint \---

The boat should only point towards the mouse pointer and move `if`{:class="block3control"} the `distance to the mouse pointer`{:class="block3sensing"} is `greater than 5 pixels`{:class="block3operators"}.

\--- /hint \--- \--- hint \---

These are the code blocks you need to add to the code for the boat sprite:

![boat-sprite](images/boat_resize.png)

```blocks3
만약 < [ ] > [ ] > 이라면

((mouse-pointer v) 쪽 보기)
```

\--- /hint \--- \--- hint \---

This is what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
녹색 깃발이 클릭되었을 때
(0) 도 방향 보기
x: (-190) y: (-150) 으로 이동하기
무한 반복하기
만약 <((마우스 포인터 v) 까지의 거리) > [5] > 이라면
(마우스 포인터 v)  쪽 보기
(1) 만큼 움직이기
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your code again to check whether the problem is now fixed.

\--- /task \---