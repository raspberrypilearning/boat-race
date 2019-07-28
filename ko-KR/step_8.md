## 장애물 및 부스터

지금 이 게임은 **지나치게** 매우 쉽습니다. - 더 재미있는 것들을 추가해봅시다.

먼저 보트 속도를 높이기 위해 몇 가지 부스터를 추가합니다.

\--- task \---

일부 흰색 부스터 화살표를 추가하여 스테이지 배경을 편집하십시오.

![screenshot](images/boat-boost.png)

\--- /task \---

\--- task \---

이제 더 많은 코드 블록을 보트의 `무한 반복`{:class="block3control"} 에 추가하세요. 보트 스프라이트가 흰색 화살표에 닿으면 3칸 앞으로 움직입니다. ![boat-sprite](images/boat_resize.png)

```blocks3
만약 <touching color [#FFFFFF] ?> 이라면
(3) 만큼 움직이기
끝
```

\--- /task \---

\--- task \---

게임을 테스트하여 새 부스터 화살이 보트 속도를 높이는 지 확인하십시오.

\--- /task \---

다음으로 배가 피해야하는 회전문을 추가합니다.

\--- task \---

다음과 같은 새 스프라이트를 추가하고 이를 'gate' 라고 부릅니다.

![스크린샷](images/boat-gate.png)

문의 색이 나무 장애물과 같은 색인지 확인하세요.

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![스크린샷](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![gate](images/gate.png)

```blocks3
forever
end

turn cw (1) degrees

when flag clicked
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

```blocks3
when flag clicked
forever
turn cw (1) degrees
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![스크린샷](images/boat-gate-test.png)

\--- /task \---