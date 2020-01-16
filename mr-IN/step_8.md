## अडथळे आणि बूस्टर

सध्या गेम **दूर** खूप सोपा आहे, म्हणून आपण त्यास अधिक मनोरंजक बनविण्यासाठी काही गोष्टी जोडाल.

प्रथम, आपण बोट गती देण्यासाठी काही बूस्टर जोडतील.

\--- कार्य \---

काही पांढर्या बूस्टर बाणांमध्ये जोडून आपला स्टेज बॅकड्रॉप संपादित करा.

![स्क्रीनशॉट](images/boat-boost.png)

\--- /task \---

\--- task \---

आता आपल्या बोटच्या `नेहमी कोड`{: class = "block3control"} लाओप जोडा जेणेकरून बोट स्प्राइट एका पांढऱ्या बाणला स्पर्श करते तेव्हा तीन अतिरिक्त चरण हलवेल.

![boat-sprite](images/boat_resize.png)

```blocks3
जर <touching color [#FFFFFF] ?> तर
हालचाली (3) चरण
समाप्त होईल
```

\--- /task \---

\--- task \---

Test your game to see whether your new booster arrows speed up the boat.

\--- /task \---

Next you'll add a spinning gate that the boat has to avoid.

\--- task \---

Add a new sprite that looks like this, and call it 'gate':

![screenshot](images/boat-gate.png)

Make sure that the colour of the gate sprite is the same as the colour of the wooden barriers.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \---

Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![gate](images/gate.png)

```blocks3
फ्लॅग क्लिक केल्यावर कायमचे
समाप्ती

CW (1) अंश

चालू करा
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
जेव्हा ध्वज
कायमचे क्लिक करेल
सीडब्ल्यू (1) अंश
अंतरावर वळवा
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---