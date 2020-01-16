## බාධක(obstacles) සහ බූස්ටර(boosters)

දැන් ක්‍රීඩාව **ඉතා(far too)** පහසු(easy) බැවින්, එය වඩාත් සිත්ගන්නා සුළු කිරීම සඳහා ඔබ එයට සමහර දේවල් එකතු කරනු ඇත.

පළමුව, ඔබ බෝට්ටුව වේගවත්(speed up) කිරීම සඳහා බූස්ටර(boosters) කිහිපයක් එකතු කරනු ඇත.

\--- task \---

සුදු(white) බූස්ටර(booster) ඊතල(arrows) කිහිපයක් එකතු කිරීමෙන් ඔබගේ වේදිකා(stage) පසුබිම(backdrop එක) සංස්කරණය(edit) කරන්න.

![තිර රුව(screenshot)](images/boat-boost.png)

\--- /task \---

\--- task \---

දැන් ඔබේ බෝට්ටුවේ `අපරිමිත{forever}`{:class="block3control"} ලූපයට(loop එකට) තවත් කේත(code) කට්ටි එකතු කිරීම මඟින් බෝට්ටු sprite එක සුදු(white) ඊතලයක්(arrow එකක්) ස්පර්ශ කරන විට එය අමතර පියවර තුනක් ඉදිරියට ගමන් කරන පරිදි සකසන්න.

![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [#FFFFFF] ?> then
move (3) steps
end
```

\--- /task \---

\--- task \---

Test your game to see whether your new booster arrows speed up the boat.

\--- /task \---

Next you'll add a spinning gate that the boat has to avoid.

\--- task \---

Add a new sprite that looks like this, and call it 'gate':

![screenshot](images/boat-gate.png)

Make sure that the colour of the gate sprite is the same as the colour of the wooden barriers.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \---

Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![gate](images/gate.png)

```blocks3
forever 
end

turn cw (1) degrees

when flag clicked
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
when flag clicked
forever
turn cw (1) degrees
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---