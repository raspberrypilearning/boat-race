## ሰዓት ቆጣሪ በማከል ላይ

አሁን ተጫዋቹ በተቻለ ፍጥነት ወደ ደሴቱ መድረስ እንዳለበት የጊዜ ማጫወቻዎን ያክላሉ.

\--- ተግባር \---

ወደ ራስዎ ደረጃ `ጊዜ`{: class = "block3variables"} የተባለ አዲስ ተለዋዋጭ ያክሉ.

![ቅጽበታዊ ገጽ እይታ](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

እንዲሁም አዲሱን ተለዋዋጭዎ እንዴት እንደሚታይ በመቀየር ሰዓት ቆጣሪዎን መፈለግ ይችላሉ.

\--- / task \---

\--- ተግባር \---

አሁን ወደ ጀልባው እስኪደርስ ድረስ የጊዜ ማቆሚያ ጊዜ ቆጣሪው እንዲቆጥብ ወደ ኮከብ ደረጃዎችዎ የቁጥር ማያያዣዎች ይጨምሩ.

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
[ጊዜ v] በ (0.1)

ጠቋሚን ጠቅ ሲያደርግ

ለዘለዓለም
መጨረሻ

ይጠብቁ (0.1) ሰከንዶች

ሴንት [ጊዜ v] እስከ [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
ባንዲራ ጠቅ ጊዜ
ወደ ስብስብ [ሰዓት v] [0]
ለዘላለም
መጠበቅ (0.1) ሰከንዶች
(0.1) በ ለውጥ [ጊዜ v]
መጨረሻ
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---