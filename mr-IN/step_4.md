## क्रॅशिंग!

या क्षणी, बोट स्प्राइट लाकडी अडथळ्यांमधून सहज जाऊ शकेल! आता आपण ते निराकरण करणार आहात.

\--- कार्य \---

आपल्या बोट स्प्राइटसाठी दोन पोशाखांची गरज आहेः एक सामान्य पोशाख आणि जेव्हा एखादी नौका क्रॅश होते तेव्हा. आपल्या बोट स्प्राइटच्या पोशाखांची नक्कल करा आणि एक पोशाख 'सामान्य' आणि इतर 'हिट' नाव द्या.

\--- / कार्य \---

\--- कार्य \---

आपल्या 'हिट' पोशाख वर क्लिक करा आणि पोशाखांचे तुकडे मिळवण्यासाठी **सिलेक्ट** टूल वापरा आणि त्यानुरूप फिरण्यासाठी आणि फिरवण्यासाठी त्यांना फिरवा.

![स्क्रीनशॉट](images/boat-hit-costume-annotated.png)

\--- / कार्य \---

\--- कार्य \---

आता आपल्या बोटमध्ये कोड जोडा जेणेकरून तो तपकिरी लाकडी अडथळ्यांना स्पर्श करेल तेव्हा तो क्रॅश होईल आणि ब्रेक होईल.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
जर <touching color [ ] ?> तर
शेवट

x वर जाईल (-190) y: (-150)

स्विच कॉस्च्यूम (हिट व्ही) वर

पॉइंट दिशेने (0)

स्विच कॉस्च्यूम (सामान्य व्ही)

म्हणा [Noooooo!] साठी (2) सेकंद
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
जेव्हा ध्वज
बिंदू दिशेने क्लिक केले (0)
x वर जा: (-190) y: (-150)
कायमचे
असल्यास <((माऊस-पॉइंटर विरुद्ध) पर्यंत अंतर > [5]> नंतर
बिंदू दिशेने (माउस- पॉईंटर v)
हलवा (1) चरणांची
ओवरनंतर
तर <touching color [#663b00] ?> नंतर
v) (दाबा स्विच पोशाख
म्हणू [Noooooo!] (2) सेकंद
(सामान्य v) स्विच पोशाख
दिशेने बिंदू (0)
x वर जा: (-190) y: (-150)
शेवटी
```

\--- /hint \--- \--- /hints \---

\--- / कार्य \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---