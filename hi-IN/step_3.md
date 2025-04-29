## नाव को नियंत्रित करना

\--- task \---

Add this code to the boat sprite so that it starts in the bottom left-hand corner pointing up and then follows the mouse pointer.

![नाव स्प्राइट](images/boat_resize.png)

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

हरे झंडे पर क्लिक करके और माउस को हिलाकर **अपने कोड का परीक्षण करें**| क्या नाव स्प्राइट माउस पॉइंटर की ओर बढ़ता है?

![स्क्रीनशॉट](images/boat-mouse.png)

\--- no-print \---

![स्क्रीनशॉट](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![स्क्रीनशॉट](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

जब आपकी नव माउस पोइंटेर तक पहुँच जाता है तब क्या होता है? अपने आप कोशिश कीजिये ताकि आप देख सकें समस्या क्या है।

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

यह जाँचने के लिए कि क्या अब समस्या ठीक हो गई है, अपने कोड का फिर एक बार परीक्षण करें।

\--- /task \---