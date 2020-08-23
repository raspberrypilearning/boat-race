## নৌকা/boat নিয়ন্ত্রণ

প্লেয়ারটি মাউসের সাহায্যে নৌকা/boat Sprite কে নিয়ন্ত্রণ করবে।.

\--- task \---

খেলা শুরুর সময় বোট sprite টি নিচে বামের দিকে থাকবে এবং খেলা শুরু হলে নৌকার সামনের দিক মাউস পয়েন্টারকে অনুসরণ করবে, এজন্য এই কোডটি ব্যবহার করতে হবে।.

![boat-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
point towards (mouse-pointer v)
move (1) steps
```

\--- /task \---

\--- task \---

**Test your code** করুন সবুজ পতাকাটি ক্লিক করে এবং মাউসটি সরিয়ে পরীক্ষা করুন। বোট sprite কি মাউস পয়েন্টারের দিকে চলে?

![screenshot](images/boat-mouse.png)

\--- no-print \---

![screenshot](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![screenshot](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

নৌকা মাউস পয়েন্টারে পৌঁছলে কী ঘটে? সমস্যাটি কী তা দেখতে চেষ্টা করুন ।.

\--- /task \---

\--- task \---

এটি বন্ধের জন্য আপনাকে এই ব্লক টি `if`{:class="block3control"} আপনার কোড এর সাথে যোগ করতে হবে, তাহলে আপনার বোট sprite মাউস পয়েন্টার থেকে 5 পিক্সেল দূরে থাকলেই এগোবে.

\--- hints \--- \--- hint \---

বোট শুধুমাত্র মাউস পয়েন্টার কেই অনুসরণ করবে এবং সরে যাবে যদি `if`{:class="block3control"} `distance to the mouse pointer`{:class="block3sensing"} is `greater than 5 pixels`{:class="block3operators"}.

\--- /hint \--- \--- hint \---

বোট sprite এর কোড এর সাথে এই কোড ব্লকগুলি যোগ করুন:

![boat-sprite](images/boat_resize.png)

```blocks3
if < [ ] > [ ] > then

(distance to (mouse-pointer v))
```

\--- /hint \--- \--- hint \---

আপনার কোড দেখতে এমন হওয়া উচিত:

![boat-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

সমস্যার সমাধান হয়েছে কিনা নিশ্চিত হওয়ার জন্য আপনার কোড টি আরেকবার পরীক্ষা করে নিন.

\--- /task \---