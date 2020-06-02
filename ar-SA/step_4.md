## الاصطدام!

في هذه اللحظة، يمكن للكائن الممثل للقارب أن يبحر عبر الحواجز الخشبية! يجب أن تقوم بحل تلك المشكلة فوراً.

\--- task \---

تحتاج إلى اثنين من مظاهر كائن القارب: واحد من مظهر عادي، والآخر من عندما يتحطم القارب. قم بتكرار مظهر كائن القارب، واسم المظهر "طبيعي" والآخر "متحطم".

\--- /task \---

\--- task \---

انقر على مظهر 'المتحطم`، و استخدم أداة ** اختيار ** لأخذ قطع من المظهر و تحريك و تدوير القارب لجعل القارب يبدو وكأنه تحطم على أجزاء.

![لقطة الشاشة](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

الآن قم بإضافة برنامج إلى قاربك بحيث يصطدم و يتحطم إلى أجزاء عندما يلامس أي حاجز خشبي بني.

\--- hints \--- \--- hint \---

تحتاج إلى إضافة كتل التعليمات البرمجية داخل حلقة `للأبد`{:class="block3control"} بحيث يستمر الكود الخاص بك في التحقق مما إذا كان كائن القارب قد تحطم، وإذا تحطم تقوم التعليمة البرمجية إلى إعادة تعيين موقع كائن القارب.

`إذا`{:class="block3control"} القارب `لمس `{:class="block3sensing"} اللون البني للخشب، تحتاج إلى `التبديل إلى المظهر المتحطم`{:class="block3looks"}، `قل كلالالالا! لمدة 2 ثانية`{:class="block3looks"}، وثم `عد إلى المظهر الطبيعي`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [ ] ?> then
end

go to x: (-190) y: (-150)

switch costume to (hit v)

point in direction (0)

switch costume to (normal v)

say [Noooooo!] for (2) seconds
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

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