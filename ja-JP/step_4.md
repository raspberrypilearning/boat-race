## ボートの制御

+ マウスでボートをコントロールします。 強調された左下隅からマウスポインタをたどるように、ボートにコードを追加します。 期待どおりに動くか**コードをテストして**確認しましょう。

-- hints \--- \--- hint \--- `緑の旗` がクリックされたらすぐにボートを `スタート地点` に移動させて `強調` する必要があります。 次に、`マウスポインタの方向を向かせ`て` 1ステップ移動する`必要があります 。 これを `永遠に` 繰り返す必要があります。

\--- /hint \--- \--- hint \--- 必要になるコードブロックはこちらです。 ![screenshot](images/boat-move-blocks.png) \--- /hint \--- \--- hint \--- コードの見本はこちらです。 ![screenshot](images/boat-move-code.png) \--- /hint \--- \--- /hints \---

+ 旗をクリックしてマウスを動かし、ボートをテストしてください。ボートはマウスに向かって航行しますか？
    
    ![screenshot](images/boat-mouse.png)
    
    ![screenshot](images/boat-pointer-test-anim.gif)

## \--- collapse \---

title: 問題がある場合 ...

## image: images/image.png

**Note:** 現在、スクラッチにはバグがあり、ボートがマウスポインターに向かって付いてこなくなることがあります。 このような場合は、`マウスのポインターへ向ける`というブロックの`マウスのポインター`をもう一度えらんでください。

![screenshot](images/boat-bug.png) \--- /collapse \---

+ ボートがマウスポインタに達するとどうなりますか？それを試してみてください。

+ そうならないように、コードに`もし…なら`のブロックを入れて、ボートがマウスから5ピクセルはなれた時だけ動くようにしましょう。

\---hints\--- \---hint\---ボートは`もし…なら`で、`マウスポインターまでの距離`が`が5ピクセルより大きい` 時だけ、マウスポインターの方向を向いて移動しなければなりません \--- /hint \--- \--- hint \--- 必要になるコードブロックはこちらです。 ![screenshot](images/boat-pointer-blocks.png) \--- /hint \--- \--- hint \--- コードの見本はこちらです。 ![screenshot](images/boat-pointer-code.png) \--- /hint \--- \--- /hints \---

+ Test out your boat again to check whether the problem has been fixed.