## ටයිමරයක්(timer එකක්) එක් කිරීම

දැන් ඔබ ඔබේ ක්‍රීඩාවට ටයිමරයක් එක් කරනු ඇත, එවිට ක්‍රීඩකයා හැකි ඉක්මනින් දිවයිනට පැමිණිය යුතුය.

\--- task \---

`වේලාව(time)`{:class="block3variables"} නමින් නව විචල්‍යයක්(variable එකක්) ඔබේ වේදිකාවට(stage) එක් කරන්න.

![තිර රුව(screenshot)](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

ඔබගේ නව(new) විචල්‍යය(variable) දර්ශනය(display) වන ආකාරය වෙනස් කිරීමෙන් ඔබට ඔබේ ටයිමරය(timer එක) සඳහා පෙනුමක්(look එකක්) තෝරා ගත හැකිය.

\--- /task \---

\--- task \---

දැන් ඔබේ වේදිකාවට(stage එකට) කේත(code) කට්ටි(blocks) එක් කරන්න, එවිට බෝට්ටුව දිවයිනට ළඟා වන තෙක් ටයිමරය(timer එක) ගණනය(count) කෙරනු ඇති.

\--- hints \--- \--- hint \--- වේදිකාවේ, `කොල(green) කොඩිය(flag එක) ක්ලික් කළ විට`{:class="block3control"}, `කාලය(time) 0 ලෙස සකසන්න(set කරන්න)`{:class="block3variables"}. ඔබේ `අපරිමිත(forever)`{:class="block3control"} ලූපය(loop එක) ඇතුළත, පළමුව ඔබට `තත්පර 0.1 ක් බලා සිටිය(wait) යුතුය`{:class="block3control}, පසුව `කාලය(time එක) 0.1 කින් වෙනස්(change) කරන්න`{:class="block3variables"}. \--- /hint \--- \--- hint \--- ඔබට අවශ්‍ය කේත(code) කට්ටි(blocks) මෙහි දැක්වේ: ![වේදිකාව](images/stage.png)

```blocks3
change [time v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [time v] to [0]
```

\--- /hint \--- \--- hint \---- ඔබේ නව(new) කේතය(code එක) මෙබඳු එකක් විය යුතුයි: ![වේදිකාව](images/stage.png)

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

ඔබේ ක්‍රීඩාව අත්හදා බලා ඔබට කෙතරම් ඉක්මනින් බෝට්ටුව දිවයිනට ගෙන යා හැකි දැයි බලන්න!

![පින්තුරය](images/boat-variable-test.png)

\--- /task \---