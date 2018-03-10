## ボートの制御

+ あなたはマウスでボートをコントロールします。 強調された左下隅からマウスポインタをたどるように、ボートにコードを追加します。 期待どおりに動くか**コードをテストして**確認しましょう。

-- hints \--- \--- hint \--- `緑の旗` がクリックされたらすぐにボートを `スタート地点` に移動させて `強調` する必要があります。 次に、`マウスポインタの方向を向かせ`て` 1ステップ移動する`必要があります 。 これを `永遠に` 繰り返す必要があります。

\--- /hint \--- \--- hint \--- Here are the code blocks you'll need: ![screenshot](images/boat-move-blocks.png) \--- /hint \--- \--- hint \--- This is what your code should look like: ![screenshot](images/boat-move-code.png) \--- /hint \--- \--- /hints \---

+ Test out your boat by clicking the flag and moving the mouse. Does the boat sail towards the mouse?
    
    ![screenshot](images/boat-mouse.png)
    
    ![screenshot](images/boat-pointer-test-anim.gif)

## \--- collapse \---

title: If you have problems ...

## image: images/image.png

**Note:** There is currently a bug in Scratch which means your boat may not move towards the mouse pointer. If this happens, click the arrow on the `point towards` block and re-select `mouse-pointer`.

![screenshot](images/boat-bug.png) \--- /collapse \---

+ What happens if the boat reaches the mouse pointer? Try it.

+ To stop this from happening, you'll need to add an `if` block to your code, so that the boat only moves if it is more than 5 pixels away from the mouse.

\--- hints \--- \--- hint \--- The boat should only point towards the mouse pointer and move `if` the `distance to the mouse pointer` is `greater than 5 pixels`. \--- /hint \--- \--- hint \--- Here are the code blocks you'll need to add to the code for the boat: ![screenshot](images/boat-pointer-blocks.png) \--- /hint \--- \--- hint \--- This is what your code should look like: ![screenshot](images/boat-pointer-code.png) \--- /hint \--- \--- /hints \---

+ Test out your boat again to check whether the problem has been fixed.