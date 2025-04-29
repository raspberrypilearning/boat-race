## নৌকা/boat নিয়ন্ত্রণ

\--- task \---

Add this code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

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

সমস্যার সমাধান হয়েছে কিনা নিশ্চিত হওয়ার জন্য আপনার কোড টি আরেকবার পরীক্ষা করে নিন.

\--- /task \---