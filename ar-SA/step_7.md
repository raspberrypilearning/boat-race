## إضافة مؤقِت

الآن سوف تضيف مؤقتاً إلى لعبتك، حتى يتمكن اللاعب من الوصول إلى الجزيرة بأسرع ما يمكن.

--- task ---

إضافة متغير جديد يسمى `الوقت`{:class="block3variables"} إلى المنصة.

![لقطة الشاشة](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

يمكنك أيضاً إضافة مظهر جديد إلى مؤقتك وذلك عن طريق تغيير كيفية عرض المتغير الجديد.

--- /task ---

--- task ---

قم بإضافة بعض التعليمات البرمجية إلى اللوحة الرئيسية بحيث يقوم المؤقت بالعد حتى يصل القارب إلى الجزيرة.

--- hints ---
 --- hint ---

على اللوحة الرئيسية `عندما يتم النقر على العلم الأخضر`{:class="block3control"}، `قم بتغيير قيمة المؤقت إلى 0`{:class="block3variables"}. داخل حلقة `forever`{:class="block3control"} ، سوف تحتاج أولاً إلى `الانتظار لمدة 0.1 ثانية`{:class="block3control"}، ومن ثم `تغيير المؤقت بمقدار 0.1 ثانية`{:class="block3variables"}.

--- /hint --- --- hint ---

هنا بعض التعليمات البرمجية التي ستحتاج إليها:

![اللوحة الرئيسية](images/stage.png)

```blocks3
change [الوقت v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [الوقت v] to [0]
```

--- /hint --- --- hint ---

هذا ما يجب أن يبدو عليه الرمز البرمجي الجديد:

![اللوحة الرئيسية](images/stage.png)

```blocks3
when flag clicked
set [الوقت v] to [0]
forever
wait (0.1) seconds
change [الوقت v] by (0.1)
end
```

--- /hint ------ /hints ---

--- /task ---

--- task ---

قم باختبار لعبتك و قم بمحاولة إيصال قاربك إلى الجزيرة بأسرع وقت ممكن!

![لقطة الشاشة](images/boat-variable-test.png)

--- /task ---