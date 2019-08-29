## ජයග්‍රහණය!

\--- task \--- දැන් බෝට්ටුව කහ(yellow) දූපතට(island එකට) පැමිණෙන විට ක්‍රීඩකයා ජය ගන්නා පරිදි, තවත් `නම්(if)`{:class="block3control"} ප්‍රකාශනයක්(statement එකක්) ඔබේ බෝට්ටු sprite ගේ කේතයට(code එකට) එකතු කරන්න.

බෝට්ටුව දිවයිනට පැමිණි විට, ක්‍රීඩාව 'යේහ්!'('YEAH!') යැයි පැවසා අවසන් විය යුතුය.

\--- hints \--- \--- hint \--- ක්‍රීඩකයා ජයග්‍රහණය කර ඇත්දැයි දිගින් දිගටම පරීක්ෂා කිරීමට ඔබේ කේතයේ(code එකේ) `අපරිමිත(forever)`{:class="block3control"} ලූපය(loop) තුළ තවත් කේත කට්ටි එකතු කළ යුතුය:

බෝට්ටුව දිවයිනේ වර්ණය `ස්පර්ශ(touching)`{:class="block3sensing"} වේ `නම්(if)`{:class="block3control"} `තත්පර 2 ක් 'යේහ්!'('YEAH!') යැයි පැවසා`{:class="block3looks"} ඉන්පසු ` සියල්ල නවත්වා(stop all)`{:class="block3control"} ක්‍රීඩාව අවසන් කල යුතුයි. \--- /hint \--- \--- hint \--- ඔබට අවශ්‍ය කේත(code) කට්ටි(blocks) මෙන්න: ![boat-sprite](images/boat_resize.png)

```blocks3
say [YEAH!] for (2) seconds

if <touching color [#FFFF99] ?> then
end 

stop [all v]

```

\--- /hint \--- \--- hint \---- ඔබේ කේතය(code එක) මෙබඳු එකක් විය යුතුයි: ![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v] 
end
```

මෙම නව කේතය `අපරිමිත(forever)`{:class="block3control"} ලූපය(loop එක) තුළ තිබිය යුතු බව අමතක නොකරන්න. \--- /hint \--- \--- /hints \--- \--- /task \---