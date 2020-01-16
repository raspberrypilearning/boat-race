## 장애물 및 부스터

현재까지 만들어진 게임은 **지나치게** 매우 쉽습니다. - 더 재미있는 것들을 추가해봅시다.

먼저 보트 속도를 높이기 위해 몇 가지 부스터를 추가합니다.

\--- task \---

스페이지 배경에 흰색 부스터 화살표를 추가하여 봅시다.

![스크린샷](images/boat-boost.png)

\--- /task \---

\--- task \---

더 많은 코드 블록을 보트의 `무한 반복`{:class="block3control"} 에 추가하세요. 흰색 화살표를 누르면 보트 스프라이트가 3칸 더 앞으로 움직입니다.

![boat-sprite](images/boat_resize.png)

```blocks3
만약 <touching color [#FFFFFF] ?> 이라면
(3) 만큼 움직이기
끝
```

\--- /task \---

\--- task \---

Test your game to see whether your new booster arrows speed up the boat.

\--- /task \---

Next you'll add a spinning gate that the boat has to avoid.

\--- task \---

Add a new sprite that looks like this, and call it 'gate':

![screenshot](images/boat-gate.png)

Make sure that the colour of the gate sprite is the same as the colour of the wooden barriers.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \---

Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![gate](images/gate.png)

```blocks3
무한 반복하기
끝

cw 방향으로 (1) 도 회전하기

flag 클릭했을 때
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
녹색 깃발을 클릭했을 때
무한 반복하기
    cw 방향으로 (1) 도 회전하기
끝
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---