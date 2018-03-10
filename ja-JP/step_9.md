## 動くかべとスピードアップ

まだまだゲームはかんたん*すぎる*ので、いろいろつけ足してもっとおもしろくしましょう。

+ まずはボートの「スピード」を上げる白いやじるしをステージに足しましょう。
    
    ![screenshot](images/boat-boost.png)

+ 白いスピードアップにふ触れたら3歩よぶんに進むように「ずっと」ループにコードを追加します。

\--- hints \--- \--- hint \--- `もし`ボートが`白いスピードアップに触れた`なら、`3歩動かす`ようにします。  
\--- /hint \--- \--- hint \--- 必要になるコードブロックはこちらです。 ![screenshot](images/boat-boost-blocks.png) \--- /hint \--- \--- hint \--- コードの見本はこちらです。 ![screenshot](images/boat-boost-code.png) \--- /hint \--- \--- /hints \---

+ ボートが避けなければならない回転するゲートを追加することもできます。次のような「gate」という新しいスプライトを追加します。
    
    ![screenshot](images/boat-gate.png)
    
    ゲートの色と木の障害物の色が同じ茶色であることをたしかめましょう。

+ ゲートスプライトを中心にセットしてください。
    
    ![screenshot](images/boat-center.png)

+ ずっとゆっくり回転するようにコードをゲートに追加します。

\--- hints \--- \--- hint \--- `ずっと``1度回す`ようなコードをゲートに追加します。 \--- /hint \--- \--- hint \--- 必要になるコードブロックはこちらです。 ![screenshot](images/boat-spin-blocks.png) \--- /hint \--- \--- hint \--- コードの見本はこちらです。 ![screenshot](images/boat-spin-code.png) \--- /hint \--- \--- /hints \---

+ ゲームをテストしましょう。避けるなければならない回転ゲートが現れるはずです。
    
    ![screenshot](images/boat-gate-test.png)