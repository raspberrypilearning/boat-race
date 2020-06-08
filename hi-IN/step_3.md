## नाव को नियंत्रित करना

खिलाड़ी माउस के साथ नाव के स्प्राइट को नियंत्रित करेगा।

--- task ---

अपनी नाव में कोड जोड़ें ताकि यह नीचे बाएँ कोने में उपर की ओर मुँह करके उस पॉइंटर का पीछा करें।

![नाव स्प्राइट](images/boat_resize.png)

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

हरे झंडे पर क्लिक करके और माउस को हिलाकर ** अपने कोड का परीक्षण करें **| क्या बोट स्प्राइट माउस पॉइंटर का पीछा कर रहा हैं?

![स्क्रीनशॉट](images/boat-mouse.png)

--- no-print ---

![स्क्रीनशॉट](images/boat-pointer-test-anim.gif)

--- /no-print ---

--- print-only ---

![स्क्रीनशॉट](images/boat-pointer-test-anim.png)

--- /print-only ---

--- /task ---

--- task ---

जब आपकी नव माउस तक पहुँच जाता हैं तब क्या होता हैं? अपने आप कोशिश कीजिये ताकि आप देख सके समस्या हैं क्या।

--- /task ---

--- task ---

ऐसा होने से रोकने के लिए, आपको अपने कोड में एक `if`{:class="block3control"} ब्लॉक शामिल करना होगा, ताकि नौका केवल तभी स्थानांतरित हो अगर यह माउस से 5 पिक्सल से अधिक दूरी पर हो।

--- hints ---
 --- hint ---

आपका नौका माउस के पॉइंटर की ओर होना और `distance to the mouse pointer`{:class="block3sensing} `if`{:class="block3control"} जब माउस पॉइंटर तक दूरी `greater than 5 pixels`{:class="block3operators"}।

--- /hint --- --- hint ---

नीचे दिए गए कोड ब्लॉक्स आपको अपने नव स्प्राइट के कोड में जोड़ना हैं।

![नाव स्प्राइट](images/boat_resize.png)

```blocks3
f < [ ] > [ ] > then

(distance to (mouse-pointer v))
```

--- /hint --- --- hint ---

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

--- /hint ------ /hints ---

--- /task ---

--- task ---

यह जाँचने के लिए कि क्या अब समस्या ठीक हो गई है, अपने कोड का फिर से एक बार परीक्षण करें।

--- /task ---