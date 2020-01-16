## በመብራት ላይ!

በአሁኑ ጊዜ የጀልባ መስመሮች በእንጨት መሰንጠቂያዎች በኩል መጓዝ ይችላሉ! አሁን ያንን ለማስተካከል ነው.

\--- ተግባር \---

ለጀልባዎ ሽፋን ሁለት ልብስ ያስፈልገዎታል: አንድ መደበኛ ልብሶች, እና አንድ ጀልባ በሚነዳበት ጊዜ አንዱ. የጀልባ ስፒርትን ልብስ ቀድቶ አንድ ቀለም «መደበኛ» እና ሌላውን «መጎዳት» የሚል ስም ይስጡ.

\--- / task \---

\--- ተግባር \---

የ "ታምር" ልብስዎ ላይ ጠቅ ያድርጉ እና የ **መሣሪያን** መሣሪያ በመጠቀም ድራቸውን ተይዘው ለመውሰድ እና ለማንቀሳቀስ እና ለማሽከርከር የችግሩን መርገጫ በመጠቀም ይጥፉ.

![ቅጽበታዊ ገጽ እይታ](images/boat-hit-costume-annotated.png)

\--- / task \---

\--- ተግባር \---

አሁን ማንኛውንም የጫጭን የእንጨት እቃዎች ሲነካው እንዲበላሸው እና እንዲበስልዎ ኮድ ወደ መርከብዎ ያክሉ.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
<touching color [ ] ?> ከዚያም
መጨረሻ

ወደ x ይሂዱ: (-190) y: (-150)

ለውጦችን ወደ (v (መጎዳቱን) v)

አቅጣጫዎችን (0)

ለውጦችን ወደ (መደበኛ ቫ)

ይቀይሩ [ኖውሞ!] ለ (2) ሰከንድ
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
ባንዲራ ጠቅ ጊዜ
አቅጣጫ ነጥብ (0)
x ሂድ: (-190) y: (-150)
ለዘላለም
ከሆነ <((መዳፊት-የጠቋሚ v) ወደ ርቀት) > [5]> ከዚያም
አቅጣጫ ነጥብ (mouse- ጠቋሚው v)
አንቀሳቅስ (1) ደረጃዎች
መጨረሻ
ቢ <touching color [#663b00] ?> ከዛ
ልብስ ይቀይሩ (v)
ይቀይሩ [noooooo!] ለ (2) ሰከንዶች
ልብሱን ወደ (መደበኛ ቪ) ይቀይሩ
አቅጣጫ ወደ (0)
ወደ x ይሂዱ: (-190) y: (-150)
መጨረሻ
```

\--- /hint \--- \--- /hints \---

\--- / task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---