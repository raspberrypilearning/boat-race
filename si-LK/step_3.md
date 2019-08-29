## බෝට්ටුව පාලනය කිරීම

ක්‍රීඩකයා(player) මූසිකය(mouse එක) මගින් බෝට්ටු sprite එක පාලනය කරනු ඇත.

\--- task \--- බෝට්ටු sprite එක වම්පස පහළ කෙළවරේ සිට ඉහළට යොමු වී ආරම්භව, මූසික(mouse) දර්ශකය(pointer එක) අනුගමනය කරන පරිදි එයට කේතයක්(code එකක්) එක් කරන්න. 

![boat-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
point towards (mouse-pointer v)
move (1) steps
```

\--- /task \---

\--- task \---

කොල ධජය(green flag එක) ක්ලික් කර මූසිකය(mouse එක) චලනය කිරීමෙන්. බෝට්ටු sprite එක මූසික(mouse) දර්ශකය(pointer එක) දෙසට ගමන් කරයිදැයි බලමින්, ** ඔබේ කේතය පරීක්ෂා කරන්න (test your code)**

![තිර රුව(screenshot)](images/boat-mouse.png)

\--- no-print \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- /no-print \---

\--- print-only \--- ![screenshot](images/boat-pointer-test-anim.png) \--- /print-only \---

\--- /task \---

\--- task \---

බෝට්ටුව(boat එක) මූසික(mouse) දර්ශකය(pointer එක) වෙත ළඟා වූ විට කුමක් සිදුවේද? ගැටලුව කුමක්දැයි බැලීමට එය උත්සාහ කරන්න.

\--- /task \---

\--- task \---

මෙය සිදුවීම වලක්වා ගැනීමට, ඔබ `නම්(if)`{:class="block3control"} කට්ටියක් ඔබේ කේතයට(code එකට) එකතු කළ යුතුය, එවිට බෝට්ටු sprite එක චලනය වන්නේ එය මූසික(mouse) දර්ශකයෙන්(Pointer එකෙන්) පික්සල්(pixels) 5 ට වඩා දුරින් ඇති විට පමණි.

\--- hints \--- \--- hint \--- බෝට්ටුවේ සිට `මූසික දර්ශකයට ඇති දුර `{:class="block3sensing"} `පික්සල් 5 ට වඩා වැඩි`{:class="block3operators"} `නම්(if)`{:class="block3control"} බෝට්ටුව මූසික දර්ශකය දෙසට පමණක් යොමුව ගමන් කළ යුතුය. \--- /hint \--- \--- hint \--- බෝට්ටු sprite එකේ කේතයට(code එකට) ඔබ එකතු කළ යුතු කේත(code) කට්ටි(blocks) මෙහි දැක්වේ: ![boat-sprite](images/boat_resize.png)

```blocks3
if < [ ] > [ ] > then
```

\--- /hint \--- \--- hint \---- ඔබේ කේතය(code එක) මෙබඳු එකක් විය යුතුයි: ![boat-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150) 
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v) 
move (1) steps
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

ගැටලුව දැන් විසඳී ඇත්දැයි පරීක්ෂා කිරීමට ඔබේ කේතය(code එක) නැවත පරීක්ෂා(test) කරන්න.

\--- /task \---