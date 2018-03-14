## 시간 제한

게임에 타이머를 추가하여, 플레이어가 가능한 빨리 무인도에 도착하게 합시다.

+ `시간` 이라는 새 변수를 무대에 추가합니다. 새 변수의 표기를 변경할 수 있습니다.
    
    ![screenshot](images/boat-variable.png)

[[[generic-scratch-add-variable]]]

+ 이제 배가 무인도에 도착할 때까지 타이머가 시간을 잴 수 있도록 무대에 코드를 추가하세요.

\--- hints \--- \--- hint \--- 무대에서, `깃발을 클릭하면`, 타이머의 `시간을 0으로 설정`합니다. Inside your `forever` block, you'll need to first `wait 0.1 secs`, then `change the time by 0.1`. \--- /hint \--- \--- hint \--- Here are the code blocks you'll need: ![screenshot](images/boat-time-blocks.png) \--- /hint \--- \--- hint \--- Here's what your code should look like: ![screenshot](images/boat-time-code.png) \--- /hint \--- \--- /hints \---

+ That's it! Test out your game and see how quickly you can get to the desert island!
    
    ![screenshot](images/boat-variable-test.png)