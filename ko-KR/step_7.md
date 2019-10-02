## 타이머 추가하기

게임에 타이머를 추가하여, 플레이어가 가능한 빨리 무인도에 도착하도록 만들어 봅시다.

--- task ---

`time`{:class="block3variables"}이라는 이름의 새 변수를 추가 해 보세요.

![스크린샷](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

새 변수가 표시되는 방식을 변경하여 타이머 모양을 변경할 수도 있습니다.

--- /task ---

--- task ---

이제 배가 무인도에 도착할 때까지 타이머가 시간을 잴 수 있도록 무대에 코드를 추가하세요.

--- hints ---
 --- hint --- 무대에서, `깃발을 클릭하면`{:class="block3control"}, 타이머의 `시간을 0으로 설정`{:class="block3variables"}합니다. `무한 반복`{:class="block3control"} 반복문 안에, `0.1 초 기다리기`{:class="block3control"} 블록을 추가하고, `time을 0.1 만큼 바꾸기`{:class="block3variables"} 블록을 추가합니다.
--- /hint ---
 --- hint --- 사용할 수 있는 코드 블럭의 종류가 아래와 같이 있어요: ![스테이지](images/stage.png)

```blocks3
[time v] 을\(를\) (0.1) 만큼 바꾸기

⚑ 클릭했을 때

무한 반복하기
end

(0.1) 초 기다리기

[time v] 을\(를\) [0] 로 정하기
```

--- /hint --- --- hint --- 아래와 같이 코드를 설계할 수 있습니다: ![스테이지](images/stage.png)

```blocks3
⚑ 클릭했을 때
[time v] 을\(를\) [0] 로 정하기
무한 반복하기 
(0.1) 초 기다리기
[time v] 을\(를\) (0.1) 만큼 바꾸기
end
```

--- /hint --- --- /hints ---

--- /task ---

--- task ---

다 됐습니다! 게임을 테스트하여 배가 무인도에 도착하는 시간을 확인해 보세요!

![스크린샷](images/boat-variable-test.png)

--- /task ---