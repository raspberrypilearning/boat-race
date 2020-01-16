## התרסקות!

כרגע, הספינה הספינה יכול פשוט להפליג דרך מחסומי עץ! אתה עומד לתקן את זה עכשיו.

\--- task \---

אתה צריך שני תלבושות עבור ספרייט הספינה שלך: אחד תלבושות נורמלי, ואחד עבור כאשר הסירה קריסות. שכפל את התלבושת הספרייט של הספינה, ואת שם אחד תחפושת 'נורמלי' והשני 'מכה'.

\--- /task \---

\--- task \---

לחץ על התלבושת 'פגע' שלך, ולהשתמש בכלי **בחר** כדי לתפוס חתיכות של תחפושת ולנוע ולסובב אותם כדי להפוך את הסירה להיראות כאילו יש התרסק לרסיסים.

![צילום מסך](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

עכשיו להוסיף קוד הסירה שלך, כך שהוא מתרסקת נשבר כאשר הוא נוגע כל מחסומי עץ חום.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
אם <touching color [ ] ?> ואז
סוף

עבור x: (-190) y: (-150)

תלבושת לעבור (פגע v)

נקודת בכיוון (0)

תלבושת 

 כדי לעבור (רגיל v)

אומר [Noooooo!] עבור (2 שניות
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
כאשר דגל לחץ על
נקודת כיוון) 0 (
עבור אל x)) -190 (y:) -150 (
לתמיד
אם <) מרחק ל (מצביע העכבר v)) > [5]> ולאחר מכן
לכיוון ( מצביע v)
(1) שלבים
בסוף
אם <touching color [#663b00] ?> ולאחר מכן
תחליף לתלבושת (v)
נניח [Noooooo!] עבור (2) שניות
תלבושת מתלבקת ל (רגילה)
נקודת כיוון (0)
עבור אל x: (-190) y: (-150)

```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---