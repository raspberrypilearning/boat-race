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

බෝට්ටුව ලී වල දුඹුරු පැහැය `ස්පර්ශ(touching)`{:class="block3sensing"} වේ `නම්(if)`{:class="block3control"}, බෝට්ටුව `hit ඇඳුමට(costume එකට)`{:class="block3looks"} මාරු වී, `තත්පර 2 ක් අයියො!(Noooo!)</0>{:class="block3looks"} යැයි පවසිය යුතුයි. පසුව <code>සාමාන්‍ය(normal) ඇඳුමට(costume එකට) මාරු වන්න`{:class="block3looks"}. අවසාන වශයෙන්, ඔබ `උඩු අතට හැරී(point up)`{:class="block3motion"} `ආරම්භක ස්ථානයට යායුතුයි`{:class="block3motion"}. පෙන්වා දීමට අවශ්‍ය වේ

\--- /hint \--- \--- hint \--- ඔබට අවශ්‍ය කේත(code) කට්ටි(blocks) මෙහි දැක්වේ:![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [ ] ?> then
end

go to x: (-190) y: (-150)

switch costume to (hit v)

point in direction (0)

switch costume to (normal v)

say [Noooooo!] for (2) seconds
```

\--- /hint \--- \--- hint \---- ඔබේ කේතය(code එක) මෙබඳු එකක් විය යුතුයි: ![boat-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150) 
forever if <(distance to (mouse-pointer v)) > [5]> then
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

ඔබේ බෝට්ටු sprite එක සෑම විටම 'සාමාන්‍ය'(normal) පෙනුමක් ඇතිව අරම්භ වන පරිදි කේතයක්(code එකක්) එකතු කළ යුතුය.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---