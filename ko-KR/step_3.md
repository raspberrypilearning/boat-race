## 배 조종하기

플레이어는 보트 스프라이트를 마우스로 제어합니다.

\--- task \--- 배가 왼쪽 아래 모퉁이에서 위를 향하여 출발하며 마우스 포인터를 따라가도록 코드를 입력합니다.

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

** 코드를 테스트하세요. ** 녹색 깃발을 클릭하고 마우스를 움직이면, 보트 스프라이트가 마우스 포인터쪽으로 이동합니까?

![스크린샷](images/boat-mouse.png)

\--- no-print \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- /no-print \---

\--- print-only \--- ![screenshot](images/boat-pointer-test-anim.png) \--- /print-only \---

\--- /task \---

\--- task \---

보트가 마우스 포인터에 도달하면 어떻게 됩니까? 문제가 무엇인지 확인해보십시오.

\--- /task \---

\--- task \---

이를 방지하려면, 배가 마우스로부터 5 픽셀보다 멀어졌을 경우에만 움직이도록 `만약` 블록을 추가해야 합니다.

\--- hints \--- \--- hint \--- 배는 오로지 마우스 포인터를 향해서 움직여야 하고 `만약`{:class="block3control"} 배에서 `마우스 포인터까지의 거리`{:class="block3sensing"}가 `5 픽셀보다 크면`{:class="block3operators"} 움직여야 합니다. \--- / hint \--- \--- 힌트 \--- 다음은 보트 스프라이트의 코드에 추가해야하는 코드 블록입니다. ![boat-sprite](images/boat_resize.png)

```blocks3
만약 < [ ] > [ ] > 이라면

((mouse-pointer v) 쪽 보기)
```

\--- /hint \--- \--- hint \--- 아래와 같이 코드를 설계할 수 있습니다: ![boat-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your code again to check whether the problem is now fixed.

\--- /task \---