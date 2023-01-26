## नाव को नियंत्रित करना

खिलाड़ी माउस के साथ नाव स्प्राइट को नियंत्रित करेगा।

\--- task \---

नाव स्प्राइट में कोड जोड़ें ताकि वह ऊपर की ओर इशारा करते हुए निचले बाएं कोने में शुरू करे और फिर माउस पॉइंटर का पीछा करें।

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

ऐसा होने से रोकने के लिए, आपको अपने कोड में एक `if`{:class="block3control"} ब्लॉक शामिल करना होगा, ताकि नाव केवल तभी चले अगर यह माउस से 5 पिक्सल से अधिक दूरी पर हो।

\--- hints \--- \--- hint \---

आपका नौका माउस के पॉइंटर की ओर होना `if`{:class="block3control"} `distance to the mouse pointer`{:class="block3sensing} है `greater than 5 pixels`{:class="block3operators"}।

\--- /hint \--- \--- hint \---

ये कोड ब्लॉक हैं जिन्हें आपको नाव स्प्राइट के कोड में जोड़ने की आवश्यकता है:

![नाव स्प्राइट](images/boat_resize.png)

```blocks3
if < [ ] > [ ] > then

(distance to (mouse-pointer v))
```

\--- /hint \--- \--- hint \---

आपका कोड ऐसा दिखना चाहिए:

![नाव स्प्राइट](images/boat_resize.png)

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

यह जाँचने के लिए कि क्या अब समस्या ठीक हो गई है, अपने कोड का फिर एक बार परीक्षण करें।

\--- /task \---