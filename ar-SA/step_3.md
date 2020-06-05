## التحكم في القارب

سيتحكم اللاعب في كائن القارب بالفأر المتصل بالحاسوب.

--- task ---

أضف برنامجاً إلى الكائن الممثل للقارب بحيث يبدأ من الزاوية السفلى اليسرى و يشير للأعلى و من ثم يتبع مؤشر الماوس.

![كائن القارب](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
point towards (mouse-pointer v)
move (1) steps
```

--- /task ---

--- task ---

 اختبار التعليمات البرمجية الخاصة بك  عن طريق النقر فوق العلم الأخضر وتحريك الماوس. هل يتحرك الكائن الممثل للقارب نحو مؤشر الماوس؟

![لقطة الشاشة](images/boat-mouse.png)

--- no-print ---

![لقطة الشاشة](images/boat-pointer-test-anim.gif)

--- /no-print ---

--- print-only ---

![لقطة الشاشة](images/boat-pointer-test-anim.png)

--- /print-only ---

--- /task ---

--- task ---

ماذا يحدث عندما يصل القارب إلى مؤشر الماوس؟ جربه لترى ما المشكلة.

--- /task ---

--- task ---

لمنع حدوث ذلك، تحتاج إلى إضافة تعليمة برمجية`if`{:class="block3control"} إلى التعليمة البرمجية الخاص بك، بحيث يتحرك كائن القارب فقط إذا كان يبعد أكثر من 5 بكسل عن مؤشر الفأر.

--- hints ---
 --- hint ---

يجب أن يشير القارب نحو مؤشر الماوس و يتحرك `إذا`{:class="block3control"} `المسافة نحو مؤشر الماوس`{:class="block3sensing"} `أكبر من 5 بكسلات`{:class="block3operators"}.

--- /hint --- --- hint ---

هذه هي التعليمات البرمجية التي تحتاج إلى إضافتها إلى التعليمات البرمجية لكائن القارب:

![كائن القارب](images/boat_resize.png)

```blocks3
if < [ ] > [ ] > then

(distance to (mouse-pointer v))
```

--- /hint --- --- hint ---

هذا ما يجب أن تبدو عليه التعليمات البرمجية الخاصة بك:

![كائن القارب](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

--- /hint ------ /hints ---

--- /task ---

--- task ---

اختبر التعليمات البرمجية الخاصة بك مرة أخرى للتحقق مما إذا كانت المشكلة قد تم إصلاحها الآن.

--- /task ---