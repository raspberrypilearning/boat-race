## מכשולים ומאיצים

עכשיו המשחק הוא **רחוק** קל מדי, כך תוכל להוסיף כמה דברים כדי לעשות את זה יותר מעניין.

ראשית, תוסיף כמה boosters כדי להאיץ את הסירה.

\--- task \---

עריכת רקע הבמה שלך על ידי הוספת כמה חיצים מגבר לבן.

![צילום מסך](images/boat-boost.png)

\--- /task \---

\--- task \---

עכשיו להוסיף עוד קוביות קוד לסירה שלך `לנצח`:: class = "block3control"} לולאה כך הספרייט הספינה נע שלושה שלבים נוספים כאשר נוגע חץ לבן. ![סירה](images/boat_resize.png)

```blocks3
אם <touching color [#FFFFFF] ?> ואז
להעביר (3) צעדים
סוף
```

\--- /task \---

\--- task \---

בדוק את המשחק שלך כדי לראות אם החצים החדשים שלך מאיץ להאיץ את הסירה.

\--- /task \---

לאחר מכן תוסיף שער מסתובב כי הסירה יש להימנע.

\--- task \---

הוסף שדון חדש שנראה כך וקרא לו 'שער':

![צילום מסך](images/boat-gate.png)

ודא כי צבע של שדון השער זהה לצבע של מחסומי עץ.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![שער](images/gate.png)

```blocks3
לנצח
סוף

הפעל cw (1) מעלות

כאשר הדגל נלחץ
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

```blocks3
כאשר דגל לחץ
לנצח
הפעל cw (1) מעלות
סוף
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---