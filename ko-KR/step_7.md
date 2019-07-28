## 타이머 추가하기

게임에 타이머를 추가하여, 플레이어가 가능한 빨리 무인도에 도착하게 합시다.

\--- task \---

`time`{:class="block3variables"}이라는 이름의 새 변수를 추가 해 보세요.

![스크린샷](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

새 변수가 표시되는 방식을 변경하여 타이머 모양을 선택할 수도 있습니다.

\--- /task \---

\--- task \---

이제 배가 무인도에 도착할 때까지 타이머가 시간을 잴 수 있도록 무대에 코드를 추가하세요.

\--- hints \--- \--- hint \--- 무대에서, `깃발을 클릭하면`{:class="block3control"}, 타이머의 `시간을 0으로 설정`{:class="block3variables"}합니다. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}. \--- /hint \--- \--- hint \--- 사용할 수 있는 코드 블럭의 종류가 아래와 같이 있어요: ![stage](images/stage.png)

```blocks3
change [time v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [time v] to [0]
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![stage](images/stage.png)

```blocks3
when flag clicked
set [time v] to [0]
forever
wait (0.1) seconds
change [time v] by (0.1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![스크린샷](images/boat-variable-test.png)

\--- /task \---