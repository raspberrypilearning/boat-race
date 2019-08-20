## 우승!

\--- task \--- 이제 다른 `만약`{: class = "block3control"} 블록을 보트 스프라이트 코드에 붙여 넣으면 배가 노란색 섬에 도착하면 플레이어가 이기게 됩니다.

배가 노란색 무인도에 닿으면 '야호!' 라고 말하고 게임이 끝나야 합니다.

\--- hints \--- \--- hint \--- 플레이어가 이겼는지 계속 확인하도록 `무한 반복하기`{:class="block3control"} 반복문을 코드에 추가합니다:

`만약`{:class="block3control"} 배가 보물섬의 `색깔에 닿았`{:class="block3sensing"}다면, `'야호!' 하고 2초동안 말하고`{:class="block3looks"}나서, 게임을 끝내기 위해 `모두 멈추기`{:class="block3control"} 블록를 실행합니다. \--- /hint \--- \--- hint \--- 다음 코드 블록을 참고하십시오.: ![보트 스프라이트](images/boat_resize.png)

```blocks3
[YEAH!] 를 (2) 초 동안 말하기

만약 <touching color [#FFFF99] ?> 이라면
끝

멈추기 [모두 v]

```

\--- /hint \--- \--- hint \--- 아래와 같이 코드를 설계할 수 있습니다: ![보트 스프라이트](images/boat_resize.png)

```blocks3
만약 <touching color [#FFFF99] ?> 이라면
[YEAH!] 를 (2) 초 동안 말하기
멈추기 [모두 v]
끝
```

새로 작성한 코드가 `무한 반복`{: class = "block3control"} 루프 안에 있어야한다는 것을 잊지 마십시오. \--- /hint \--- \--- /hints \--- \--- /task \---