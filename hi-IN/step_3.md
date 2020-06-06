## Controlling the boat

The player will control the boat sprite with the mouse.

\--- task \---

Add code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

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

हरे झंडे पर क्लिक करके और माउस को हिलाकर ** अपने कोड का परीक्षण करें **| क्या बोट स्प्राइट माउस पॉइंटर का पीछा कर रहा हैं?

![screenshot](images/boat-mouse.png)

\--- no-print \---

![screenshot](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![screenshot](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

What happens when the boat reaches the mouse pointer? Try it out to see what the problem is.

\--- /task \---

\--- task \---

ऐसा होने से रोकने के लिए, आपको अपने कोड में एक `if`{:class="block3control"} ब्लॉक शामिल करना होगा, ताकि नौका केवल तभी स्थानांतरित हो अगर यह माउस से 5 पिक्सल से अधिक दूरी पर हो।

\--- hints \--- \--- hint \---

आपका नौका माउस के पॉइंटर की ओर होना और `distance to the mouse pointer`{:class="block3sensing} `if`{:class="block3control"} जब माउस पॉइंटर तक दूरी `greater than 5 pixels`{:class="block3operators"}।

\--- /hint \--- \--- hint \---

These are the code blocks you need to add to the code for the boat sprite:

![boat-sprite](images/boat_resize.png)

```blocks3
if < [ ] > [ ] > then

(distance to (mouse-pointer v))
```

\--- /hint \--- \--- hint \---

This is what your code should look like:

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

Test your code again to check whether the problem is now fixed.

\--- /task \---