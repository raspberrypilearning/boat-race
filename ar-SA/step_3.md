## التحكم في القارب

\--- task \---

Add this code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![كائن القارب](images/boat_resize.png)

```blocks3
عندما تنقر العلم
نقطة في الاتجاه (0)
انتقل إلى (x: (-190) y: (-150
إلى الأبد
نقطة باتجاه (مؤشر الماوس v)
تحرك خطوة واحدة
```

\--- /task \---

\--- task \---

** اختبار التعليمات البرمجية الخاصة بك ** عن طريق النقر فوق العلم الأخضر وتحريك الماوس. هل يتحرك الكائن الممثل للقارب نحو مؤشر الماوس؟

![لقطة الشاشة](images/boat-mouse.png)

\--- no-print \---

![لقطة الشاشة](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![لقطة الشاشة](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

ماذا يحدث عندما يصل القارب إلى مؤشر الماوس؟ جربه لترى ما المشكلة.

\--- /task \---

\--- task \---

Add code to the boat sprite so it only point towards the mouse pointer and moves `if`{:class="block3control"} the `distance to the mouse pointer`{:class="block3sensing"} is `greater than 5 pixels`{:class="block3operators"}.

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
+if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

\--- /task \---

\--- task \---

اختبر التعليمات البرمجية الخاصة بك مرة أخرى للتحقق مما إذا كانت المشكلة قد تم إصلاحها الآن.

\--- /task \---