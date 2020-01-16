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

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
change [time v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [time v] to [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

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

![screenshot](images/boat-variable-test.png)

\--- /task \---