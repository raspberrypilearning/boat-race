## බාධක(obstacles) සහ බූස්ටර(boosters)

දැන් ක්‍රීඩාව **ඉතා(far too)** පහසු(easy) බැවින්, එය වඩාත් සිත්ගන්නා සුළු කිරීම සඳහා ඔබ එයට සමහර දේවල් එකතු කරනු ඇත.

පළමුව, ඔබ බෝට්ටුව වේගවත්(speed up) කිරීම සඳහා බූස්ටර(boosters) කිහිපයක් එකතු කරනු ඇත.

\--- task \---

සුදු(white) බූස්ටර(booster) ඊතල(arrows) කිහිපයක් එකතු කිරීමෙන් ඔබගේ වේදිකා(stage) පසුබිම(backdrop එක) සංස්කරණය(edit) කරන්න.

![තිර රුව(screenshot)](images/boat-boost.png)

\--- /task \---

\--- task \---

දැන් ඔබේ බෝට්ටුවේ `අපරිමිත{forever}`{:class="block3control"} ලූපයට(loop එකට) තවත් කේත(code) කට්ටි එකතු කිරීම මඟින් බෝට්ටු sprite එක සුදු(white) ඊතලයක්(arrow එකක්) ස්පර්ශ කරන විට එය අමතර පියවර තුනක් ඉදිරියට ගමන් කරන පරිදි සකසන්න. ![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [#FFFFFF] ?> then
move (3) steps
end
```

\--- /task \---

\--- task \---

ඔබගේ නව බූස්ටර(booster) ඊතල(arrows) බෝට්ටුව වේගවත්(speed up) කරන්නේ දැයි බැලීමට ඔබගේ ක්‍රීඩාව පරීක්ෂා(test) කරන්න.

\--- /task \---

ඊළඟට ඔබ බෝට්ටුව මඟ හැරිය යුතු භ්‍රමණය(spinning) වන ගේට්ටුවක්(gate එකක්) එක් කරයි.

\--- task \---

මේ ආකාරයට පෙනෙන නව(new) sprite එකක් එකතු කර එය 'ගේට්ටුව'('gate') ලෙස නම් කරන්න:

![තිර රුව(screenshot)](images/boat-gate.png)

ගේට්ටු sprite එකේ වර්ණය ලී(wooden) බාධකවල(barriers වල) වර්ණයට සමාන බව තහවුරු කරගන්න.

\--- /task \---

\--- task \---

ගේට්ටු sprite එකේ කේන්ද්‍රය(centre) මධ්‍යයේ ස්ථානගත කර ඇති බවට වග බලා ගන්න.

![තිර රුව(screenshot)](images/boat-center.png)

\--- /task \---

\--- task \---

ඔබේ ගේට්ටු sprite එක දිගටම කැරකෙන ලෙස කේතයක්(code එකක්) එක් කරන්න.

\--- hints \--- \--- hint \--- ගේට්ටු sprite එක `අංශක(degree) 1 බැගින්`{:class="block3motion"} `සදහටම(forever)`{:class="block3control"} භ්‍රමනය වන පරිදි කේත කට්ටි එයට එකතු කරන්න. \--- /hint \--- \--- hint \--- ඔබට අවශ්‍ය කේත(code) කට්ටි(blocks) මෙහි දැක්වේ: ![ගේට්ටුව](images/gate.png)

```blocks3
forever 
end

turn cw (1) degrees

when flag clicked
```

\--- /hint \--- \--- hint \---- ඔබේ නව(new) කේතය(code එක) මෙබඳු එකක් විය යුතුයි: ![ගේට්ටුව](images/gate.png)

```blocks3
when flag clicked
forever
turn cw (1) degrees
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

ඔබගේ ක්‍රීඩාව නැවත පරීක්ෂා කරන්න. එහි දැන් මගහැර යායුතු භ්‍රමණය වන ගේට්ටුවක් තිබිය යුතුයි.

![තිර රුව(screenshot)](images/boat-gate-test.png)

\--- /task \---