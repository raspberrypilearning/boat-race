## הוספת טיימר

עכשיו תוסיף טיימר למשחק שלך, כך השחקן צריך להגיע לאי במהירות האפשרית.

\--- task \---

הוסף משתנה חדש הנקרא `שעה`{: class = "block3variables"} לשלב שלך.

![צילום מסך](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

תוכל גם לבחור לחפש את הטיימר שלך על ידי שינוי אופן הצגת המשתנה החדש.

\--- /task \---

\--- task \---

עכשיו להוסיף בלוקים קוד הבמה שלך, כך טיימר סופרת עד הסירה מגיע אל האי.

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
(0.1)

כאשר דגל נלחץ

לנצח
סוף

לחכות (0.1) שניות

בחר [זמן v] ל [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
כאשר דגל לחץ
קבע [זמן] ל [0]
לנצח
לחכות (0.1) שניות
שינוי [זמן v] על ידי (0.1)
סוף
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---