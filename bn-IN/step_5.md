## বিজয়!

--- task ---

এখন বোট sprita এর কোড এ আরেকটু কোড ব্লক `if`{:class="block3control"} যোগ করতে হবে যাতে খেলোয়াড়রা বিজয়ী হবেন যখন তার বোট হলুদ দ্বীপ স্পর্শ করে.

যখন নৌকা হলুদ দ্বীপে পৌঁছাবে তখন স্ক্রীনে 'YEAH!' দেখাবে এবং খেলা শেষ হয়ে যাবে।.

--- hints ---
 --- hint ---

আপনাকে আপনার আরও কোড ব্লক যুক্ত করতে হবে `forever`{:class="block3control"} লুপ এর মধ্যে যাতে আপনার কোডটি প্লেয়ারটি জিতেছে কিনা তা পরীক্ষা করতে থাকে:

`if`{:class="block3control"} বোট `touching`{:class="block3sensing"} হলুদ রঙের দ্বীপ, আপনাকে বলতে হবে `'YEAH!' for 2 seconds`{:class="block3looks"} আর তারপরে `stop all`{:class="block3control"} খেলা শেষ হয়ে যাবে.

--- /hint --- --- hint ---

আপনার প্রয়োজনীয় কোড ব্লক গুলি হলো:

![boat-sprite](images/boat_resize.png)

```blocks3
say [YEAH!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

--- /hint --- --- hint ---

আপনার নতুন কোডটি দেখতে এমন হওয়া উচিত:

![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
```

অবশ্যই মনে রাখবেন যে এই নতুন কোডটি `forever`{:class="block3control"} লুপের মধ্যে থাকা দরকার।.

--- /hint --- --- /hints --- --- /task ---