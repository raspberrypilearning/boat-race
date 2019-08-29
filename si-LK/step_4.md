## හැප්පීම!

මේ මොහොත වනවිට, බෝට්ටු sprite එකට ලී(wooden) බාධක(barriers) හරහා යාත්‍රා කළ හැකිය! ඔබට දැන් එය නිවැරදි කිරීමට හැකියි.

\--- task \---

ඔබේ බෝට්ටු sprite එක සඳහා ඔබට ඇඳුම්(costume) දෙකක් අවශ්‍යයි: එක් සාමාන්‍ය(normal) ඇඳුමක්(costume එකක්), බෝට්ටුව අනතුරට පත්වූ විට තවත් එකක්. ඔබේ බෝට්ටු sprite ගේ ඇඳුම(costume එක) අනුපිටපත්(copy) කරන්න, එක් ඇඳුමක්(costume එකක්) 'normal' සහ අනෙක 'hit' ලෙස නම් කරන්න.

\--- /task \---

\--- task \---

ඔබගේ 'hit' ඇඳුම(costume එක) මත ක්ලික් කර **තෝරන්න(Select)** මෙවලම(tool එක) භාවිතාකර ඇඳුමේ(costume එකේ) කැබලි(pieces) අල්ලාගෙන බෝට්ටුව කැබලිවලට කඩා වැටී ඇති බව පෙනෙන්නට ඒවා ගෙනයාම සහ කරකැවීම සිදු කරන්න.

![පින්තුරය](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

දැන් ඔබේ බෝට්ටුව දුඹුරු පැහැති ලී(wooden) බාධක(barriers) ස්පර්ශ වන විට හැප්පි කඩා වැටෙන පරිදි කේතයක්(code එකක්) එක් කරන්න.

\--- hints \--- \--- hint \--- ඔබේ කේතය මඟින් බෝට්ටු sprite එක හැප්පී ඇත්දැයි නිරතුරුව පරීක්ෂා කර බලන පරිදි `අනන්ත ලුපය(forever loop එක)`{:class="block3control"} තුළට කේත කට්ටි එකතු කළ යුතුය, එය හැප්පී ඇත්නම්, කේතය මගින් බෝට්ටු(boat) sprite එකේ පිහිටුම් ස්ථානය(position) නැවත සකස්(reset) කළ යුතුය.

බෝට්ටුව ලී වල දුඹුරු පැහැය `ස්පර්ශ(touching)`{:class="block3sensing"} වේ `නම්(if)`{:class="block3control"}, බෝට්ටුව `hit ඇඳුමට(costume එකට)`{:class="block3looks"} මාරු වී, `තත්පර 2 ක් අයියො!(Noooo!)</0>{:class="block3looks"} යැයි පවසිය යුතුයි. for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \--- Here are the code blocks you need: ![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [ ] ?> then
end

go to x: (-190) y: (-150)

switch costume to (hit v)

point in direction (0)

switch costume to (normal v)

say [Noooooo!] for (2) seconds
```

\--- /hint \--- \--- hint \--- Here's what your code should look like: ![boat-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
end
if <touching color [#663b00] ?> then
switch costume to (hit v)
say [Noooooo!] for (2) seconds
switch costume to (normal v)
point in direction (0)
go to x: (-190) y: (-150)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---