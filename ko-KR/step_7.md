## 타이머 추가하기

게임에 타이머를 추가하여, 플레이어가 가능한 빨리 무인도에 도착하도록 만들어 봅시다.

\--- task \---

`time`{:class="block3variables"}이라는 이름의 새 변수를 추가 해 보세요.

![스크린샷](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

새 변수가 표시되는 방식을 변경하여 타이머 모양을 변경할 수도 있습니다.

\--- /task \---

\--- task \---

이제 배가 무인도에 도착할 때까지 타이머가 시간을 잴 수 있도록 무대에 코드를 추가하세요.

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
[time v] 을 (0.1) 만큼 바꾸기

녹색 깃발을 클릭했을 때

무한 반복
끝

(0.1) 초 기다리기

[time v]를 [0] 로 정하기
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
녹색 깃발을 클릭했을 때
[time v] 을 [0] 로 정하기
무한 반복
(0.1) 초 기다리기
[time v] 을 (0.1) 만큼 바꾸기
끝
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---